---
name: smilei-index
description: This skill should be used when users ask how to use smilei and the correct generated documentation skill must be selected before going deeper into source code.
---

# smilei Skills Index

## Route the request
- Classify the request into one of the generated topic skills listed below.
- Prefer abstract, workflow-level guidance for large scientific packages; do not attempt full function-by-function coverage unless explicitly requested.

## Generated topic skills
- `smilei-validation`: Validation (documentation grouped under the 'validation' theme)
- `smilei-getting-started`: Getting Started (initial setup, quickstarts, and core concepts)
- `smilei-parallel-hpc`: Parallel and HPC (MPI/OpenMP/GPU execution, scaling, and batch systems)
- `smilei-inputs-and-modeling`: Inputs and Modeling (inputs, system setup, models, and physical parameterization)
- `smilei-build-and-install`: Build and Install (build, installation, compilation, and environment setup)
- `smilei-simulation-workflows`: Simulation Workflows (simulation setup, execution flow, and runtime controls)
- `smilei-theory-and-methods`: Theory and Methods (theoretical background and algorithmic methods)
- `smilei-troubleshooting`: Troubleshooting (known issues, diagnostics, and debugging patterns)
- `smilei-api-and-scripting`: API and Scripting (language bindings, APIs, and programmatic interfaces)
- `smilei-sphinx`: Sphinx (documentation grouped under the 'sphinx' theme)
- `smilei-benchmarks`: Benchmarks (documentation grouped under the 'benchmarks' theme)
- `smilei-font`: Font (documentation grouped under the 'font' theme)

## Documentation-first inputs
- `doc`

## Tutorials and examples roots
- `benchmarks`

## Test roots for behavior checks
- `benchmarks`
- `validation`

## Escalate only when needed
- Start from topic skill primary references.
- If those references are insufficient, search the topic skill `references/doc_map.md`.
- If documentation still leaves ambiguity, open `references/source_map.md` inside the same topic skill and inspect the suggested source entry points.
- Use targeted symbol search while inspecting source (e.g., `rg -n "<symbol_or_keyword>" happi src`).

## Source directories for deeper inspection
- `happi`
- `src`
