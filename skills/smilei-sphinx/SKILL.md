---
name: smilei-sphinx
description: This skill should be used when users ask about sphinx in smilei; it prioritizes documentation references and then source inspection only for unresolved details.
---

# smilei: Sphinx

## Scope
- Handle questions about documentation grouped under the 'sphinx' theme.
- Keep responses abstract and architectural for large codebases; avoid exhaustive per-function documentation unless requested.

## Primary documentation references
- `doc/Sphinx/index.rst`
- `doc/Sphinx/Understand/units.rst`
- `doc/Sphinx/Use/laser_offset.rst`
- `doc/Sphinx/Use/contribute.rst`
- `doc/Sphinx/site.rst`
- `doc/Sphinx/Use/particle_initialization.rst`
- `doc/Sphinx/use.rst`
- `doc/Sphinx/understand.rst`
- `doc/Sphinx/Use/maxwell-juttner.rst`
- `doc/Sphinx/Use/ids.rst`
- `doc/Sphinx/Use/binning_units.rst`
- `doc/Sphinx/Understand/physics_modules.rst`

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
- `src/ElectroMagnSolver/PML_SolverAM_EnvelopeReducedDispersion.h`
- `src/ElectroMagnSolver/PML_SolverAM_EnvelopeReducedDispersion.cpp`
- `src/ElectroMagnSolver/PML_SolverAM_Envelope.h`
- `src/ElectroMagnSolver/PML_SolverAM_Envelope.cpp`
- `src/ElectroMagnSolver/PML_SolverAM.h`
- `src/ElectroMagnSolver/PML_SolverAM.cpp`
- `src/ElectroMagnSolver/PML_Solver3D_Yee.h`
- `src/ElectroMagnSolver/PML_Solver3D_Yee.cpp`
- Prefer targeted source search (for example: `rg -n "<symbol_or_keyword>" happi src`).
