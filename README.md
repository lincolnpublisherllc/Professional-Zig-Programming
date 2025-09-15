Professional Zig Programming — Code Extraction Bundle

This repository contains only executable and configuration code extracted from the manuscript Professional Zig Programming SERIES 3, organized chapter-by-chapter. All prose has been omitted except for inline comments that appeared inside code blocks.

What’s inside

Chapters processed: 16 (INTRODUCTION + Chapters 1–15)

Chapters with code: 16

Total snippets: 345

Deduping: Identical snippets within the same chapter were removed

Whitespace fidelity: Indentation and line breaks preserved exactly

Each chapter is a folder (e.g., INTRODUCTION/, Chapter 1/, …). Files are named using:

<chapter_normalized>_snippet_<running_number>.<ext>
# examples:
# chapter_01_snippet_1.zig
# chapter_01_snippet_2.sh
# chapter_01_snippet_3.yml


Language/extension detection (heuristic):

Zig → .zig (signals: pub fn, @import, std.debug.print, comptime)

Shell/CLI → .sh (signals: zig build, git, curl, brew, sudo, etc.)

YAML → .yml (workflow-like keys: name:, on:, jobs:, steps:, etc.)

SQL → .sql (signals: SELECT, INSERT, CREATE TABLE, …)

JSON/XML when applicable

Fallback generic → .carbon (code-like but unknown language)

If a chapter had no code, a single *_placeholder.txt is created stating that no executable/config content was detected.

Quick navigation (preview)

Below is a short, human-readable index. Open each chapter folder to see the complete list of snippet files.

INTRODUCTION/

Example files: introduction_snippet_1.zig, introduction_snippet_2.zig

Chapter 1/

Example files: chapter_01_snippet_1.sh, chapter_01_snippet_2.sh, chapter_01_snippet_3.yml, …

Chapter 2/

Zig, shell, and generic snippets

Chapter 3

Chapter 4

Chapter 5

Chapter 6

Chapter 7

Chapter 8

Chapter 9

Chapter 10

Chapter 11

Chapter 12

Chapter 13

Chapter 14

Chapter 15

(Preview is truncated for readability; see chapter folders for the full file lists.)

manifest.json

A machine-readable index accompanies the bundle with per-snippet metadata.

{
  "book_title": "Professional Zig Programming SERIES 3 (code extract)",
  "chapters": [
    {
      "name": "Chapter 1",
      "snippets": [
        {
          "file": "chapter_01_snippet_1.zig",
          "language": "zig",
          "lines": 37,
          "sha256": "…",
          "summary": "One-sentence hint drawn from the preceding context."
        }
      ],
      "placeholders": 0
    }
  ]
}


Fields

file: filename relative to its chapter folder

language: detected language label (e.g., zig, bash, yml)

lines: line count (including blank lines)

sha256: hash of exact file bytes for integrity checks

summary: short hint derived from nearby manuscript context

Guarantees & constraints

No explanatory prose outside comment syntax appears in code files.

Contiguous “code-looking” lines were merged into a single snippet while preserving order.

Byte-identical snippets within a chapter were deduplicated (first occurrence kept).

Indentation and whitespace are preserved exactly (no auto-formatting done).

Suggested workflows

Search by language: glob by extension (e.g., **/*.zig) to review Zig-only samples.

Recreate examples: open chapter folders sequentially to follow the book’s teaching flow.

Integrity checks: verify file hashes against manifest.json after transfers or edits.
