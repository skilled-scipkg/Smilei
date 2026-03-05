---
name: smilei-parallel-hpc
description: This skill should be used when users ask about parallel and hpc in smilei; it prioritizes documentation references and then source inspection only for unresolved details.
---

# smilei: Parallel and HPC

## Scope
- Handle questions about MPI/OpenMP/GPU execution, scaling, and batch systems.
- Keep responses abstract and architectural for large codebases; avoid exhaustive per-function documentation unless requested.

## Primary documentation references
- `benchmarks/gpu/README.md`
- `doc/Sphinx/Understand/vectorization.rst`
- `doc/Sphinx/Understand/GPU_offloading.rst`
- `validation/references/tst3d_gpu_o2_thin_foil.py.txt`
- `validation/references/tst3d_gpu_o2_thermal_plasma_short.py.txt`
- `validation/references/tst3d_gpu_o2_thermal_plasma_medium.py.txt`
- `validation/references/tst3d_gpu_o2_thermal_plasma.py.txt`
- `validation/references/tst2d_gpu_o2_beam_plasma.py.txt`
- `doc/Sphinx/Use/optimization_flags.rst`
- `doc/Sphinx/Use/GPU_version.rst`
- `doc/Sphinx/Understand/performances.rst`

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
- `happi/_Diagnostics/Performances.py`
- `src/Tools/gpu.h`
- `src/Tools/gpu.cpp`
- `src/Diagnostic/DiagnosticPerformances.h`
- `src/Diagnostic/DiagnosticPerformances.cpp`
- `src/SmileiMPI/SmileiMPI.h`
- `src/SmileiMPI/SmileiMPI.cpp`
- `src/SmileiMPI/SmileiMPI_test.h`
- Prefer targeted source search (for example: `rg -n "<symbol_or_keyword>" happi src`).
