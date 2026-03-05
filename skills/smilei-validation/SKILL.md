---
name: smilei-validation
description: This skill should be used when users ask about validation in smilei; it prioritizes documentation references and then source inspection only for unresolved details.
---

# smilei: Validation

## Scope
- Handle questions about documentation grouped under the 'validation' theme.
- Keep responses abstract and architectural for large codebases; avoid exhaustive per-function documentation unless requested.

## Primary documentation references
- `validation/references/tstAM_17_plasma_channel_terzani.py.txt`
- `validation/references/tstAM_13_electron_sphere_field_initialization.py.txt`
- `validation/references/tst2d_13_envelope_wake.py.txt`
- `validation/references/tst2d_00_em_propagation.py.txt`
- `validation/references/tst_collisions3_AM_uniformity.py.txt`
- `validation/references/tstAM_08_envelope_wake_reduced_dispersion.py.txt`
- `validation/references/tstAM_06_envelope_wake.py.txt`
- `validation/references/tstAM_05_envelope_propagation.py.txt`
- `validation/references/tstAM_04b_laser_propagation_numpy.py.txt`
- `validation/references/tst3d_v_08_envelope_wake.py.txt`
- `validation/references/tst3d_17_envelope_wake_reduced_dispersion.py.txt`
- `validation/references/tst3d_08_envelope_wake.py.txt`

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
- `src/Field/Field3D.h`
- `src/Field/Field3D.cpp`
- `src/Field/Field2D.h`
- `src/Field/Field2D.cpp`
- `src/Field/cField3D.h`
- `src/Field/cField3D.cpp`
- `src/Field/cField2D.h`
- `src/Field/cField2D.cpp`
- Prefer targeted source search (for example: `rg -n "<symbol_or_keyword>" happi src`).
