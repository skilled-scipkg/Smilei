---
name: smilei-api-and-scripting
description: This skill should be used when users ask about api and scripting in smilei; it prioritizes documentation references and then source inspection only for unresolved details.
---

# smilei: API and Scripting

## Scope
- Handle questions about language bindings, APIs, and programmatic interfaces.
- Keep responses abstract and architectural for large codebases; avoid exhaustive per-function documentation unless requested.

## Primary documentation references
- `doc/Sphinx/Use/profiles.rst`

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
- `src/Profiles/Function.h`
- `src/Profiles/Function.cpp`
- `src/picsar_interface/interface.h`
- `src/picsar_interface/interface.cpp`
- `src/Python/pyprofiles.py`
- `src/Profiles/Profile.h`
- `src/Profiles/Profile.cpp`
- `src/Tools/userFunctions.h`
- Prefer targeted source search (for example: `rg -n "<symbol_or_keyword>" happi src`).
