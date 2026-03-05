---
name: smilei-font
description: This skill should be used when users ask about font in smilei; it prioritizes documentation references and then source inspection only for unresolved details.
---

# smilei: Font

## Scope
- Handle questions about documentation grouped under the 'font' theme.
- Keep responses abstract and architectural for large codebases; avoid exhaustive per-function documentation unless requested.

## Primary documentation references
- `doc/font/OFL.txt`

## Workflow
- Start with the primary references above.
- If details are missing, inspect `references/doc_map.md` for the complete topic document list.
- Use tutorials/examples as executable usage patterns when available.
- Use tests as behavior or regression references when available.
- If ambiguity remains after docs, inspect `references/source_map.md` and start with the ranked source entry points.
- Cite exact documentation file paths in responses.

## Tutorials and examples
- `benchmarks`

## Test references
- `benchmarks`
- `validation`

## Optional deeper inspection
- `happi`
- `src`

## Source entry points for unresolved issues
- `src/Smilei.h`
- `src/Smilei.cpp`
- `happi/__init__.py`
- `happi/_SmileiSimulation.py`
- `src/SmileiMPI/SmileiMPI.h`
- `src/SmileiMPI/SmileiMPI.cpp`
- `happi/_Utils.py`
- `happi/_Factories.py`
- Prefer targeted source search (for example: `rg -n "<symbol_or_keyword>" happi src`).
