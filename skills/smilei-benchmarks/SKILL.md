---
name: smilei-benchmarks
description: This skill should be used when users ask about benchmarks in smilei; it prioritizes documentation references and then source inspection only for unresolved details.
---

# smilei: Benchmarks

## Scope
- Handle questions about documentation grouped under the 'benchmarks' theme.
- Keep responses abstract and architectural for large codebases; avoid exhaustive per-function documentation unless requested.

## Primary documentation references
- `benchmarks/collisions/README.txt`

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
- `src/Collisions/NuclearReactionProducts.h`
- `src/Collisions/Collisions.h`
- `src/Collisions/Collisions.cpp`
- `src/Collisions/CollisionalNuclearReaction.h`
- `src/Collisions/CollisionalNuclearReaction.cpp`
- `src/Collisions/CollisionalIonization.h`
- `src/Collisions/CollisionalIonization.cpp`
- `src/Collisions/CollisionalFusionDD.h`
- Prefer targeted source search (for example: `rg -n "<symbol_or_keyword>" happi src`).
