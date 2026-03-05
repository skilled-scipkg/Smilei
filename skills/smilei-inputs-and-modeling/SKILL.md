---
name: smilei-inputs-and-modeling
description: This skill should be used when users ask about inputs and modeling in smilei; it prioritizes documentation references and then source inspection only for unresolved details.
---

# smilei: Inputs and Modeling

## Scope
- Handle questions about inputs, system setup, models, and physical parameterization.
- Keep responses abstract and architectural for large codebases; avoid exhaustive per-function documentation unless requested.

## Primary documentation references
- `doc/Sphinx/syntax_changes.rst`
- `doc/Sphinx/Understand/multiphoton_Breit_Wheeler.rst`
- `doc/Sphinx/Understand/radiation_loss.rst`
- `doc/Sphinx/Understand/laser_envelope.rst`
- `doc/Sphinx/Understand/ionization.rst`
- `doc/Sphinx/Understand/azimuthal_modes_decomposition.rst`
- `doc/Sphinx/Understand/algorithms.rst`

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
- `src/Ionization/IonizationTunnelEnvelopeAveraged.h`
- `src/Ionization/IonizationTunnelEnvelopeAveraged.cpp`
- `src/MultiphotonBreitWheeler/MultiphotonBreitWheelerTablesDefault.h`
- `src/MultiphotonBreitWheeler/MultiphotonBreitWheelerTablesDefault.cpp`
- `src/MultiphotonBreitWheeler/MultiphotonBreitWheelerTables.h`
- `src/MultiphotonBreitWheeler/MultiphotonBreitWheelerTables.cpp`
- `src/MultiphotonBreitWheeler/MultiphotonBreitWheelerFactory.h`
- `src/MultiphotonBreitWheeler/MultiphotonBreitWheeler.h`
- Prefer targeted source search (for example: `rg -n "<symbol_or_keyword>" happi src`).
