---
name: smilei-theory-and-methods
description: This skill should be used when users ask about theory and methods in smilei; it prioritizes documentation references and then source inspection only for unresolved details.
---

# smilei: Theory and Methods

## Scope
- Handle questions about theoretical background and algorithmic methods.
- Keep responses abstract and architectural for large codebases; avoid exhaustive per-function documentation unless requested.

## Primary documentation references
- `doc/Sphinx/Understand/particle_merging.rst`
- `doc/Sphinx/Understand/relativistic_fields_initialization.rst`
- `doc/Sphinx/Understand/particle_injector.rst`

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
- `src/Particles/Particle.h`
- `src/Particles/Particle.cpp`
- `src/Merging/MergingVranicSpherical.h`
- `src/Merging/MergingVranicSpherical.cpp`
- `src/Merging/MergingVranicCartesian.h`
- `src/Merging/MergingVranicCartesian.cpp`
- `src/Merging/MergingFactory.h`
- `src/Merging/Merging.h`
- Prefer targeted source search (for example: `rg -n "<symbol_or_keyword>" happi src`).
