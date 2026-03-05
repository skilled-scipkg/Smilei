---
name: smilei-simulation-workflows
description: This skill should be used when users ask about simulation workflows in smilei; it prioritizes documentation references and then source inspection only for unresolved details.
---

# smilei: Simulation Workflows

## Scope
- Handle questions about simulation setup, execution flow, and runtime controls.
- Keep responses abstract and architectural for large codebases; avoid exhaustive per-function documentation unless requested.

## Primary documentation references
- `doc/Sphinx/Use/run.rst`
- `doc/Sphinx/Use/post-processing.rst`
- `doc/Sphinx/Use/namelist.rst`
- `doc/Sphinx/Use/troubleshoot.rst`

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
- `happi/_SmileiSimulation.py`
- `src/Tools/Timers.h`
- `src/Tools/Timers.cpp`
- `src/Tools/Timer.h`
- `src/Tools/Timer.cpp`
- `src/PartCompTime/PartCompTimeFactory.h`
- `src/PartCompTime/PartCompTimeAM2Order.h`
- `src/PartCompTime/PartCompTimeAM2Order.cpp`
- Prefer targeted source search (for example: `rg -n "<symbol_or_keyword>" happi src`).
