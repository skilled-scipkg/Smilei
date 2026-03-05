---
name: smilei-build-and-install
description: This skill should be used when users ask about build and install in smilei; it prioritizes documentation references and then source inspection only for unresolved details.
---

# smilei: Build and Install

## Scope
- Handle questions about build, installation, compilation, and environment setup.
- Keep responses abstract and architectural for large codebases; avoid exhaustive per-function documentation unless requested.

## Primary documentation references
- `doc/Sphinx/Use/tables.rst`
- `doc/Sphinx/Use/installation.rst`
- `doc/Sphinx/Use/install_supercomputer.rst`
- `doc/Sphinx/Use/install_linux.rst`
- `doc/Sphinx/Use/install_macos.rst`
- `doc/Sphinx/Use/install_linux_GPU.rst`

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
- `src/Tools/gpu.h`
- `src/Tools/gpu.cpp`
- `src/Tools/userFunctions.h`
- `src/Tools/gpuRandom.h`
- `src/Radiation/RadiationTablesDefault.h`
- `src/Radiation/RadiationTablesDefault.cpp`
- `src/Radiation/RadiationTables.h`
- `src/Radiation/RadiationTables.cpp`
- Prefer targeted source search (for example: `rg -n "<symbol_or_keyword>" happi src`).
