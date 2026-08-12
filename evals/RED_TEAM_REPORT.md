# V0.1 Red-Team Smoke Report

Date: 2026-08-12

## Result

- Final red-team smoke cases: **8/8 PASS**
- Critical findings remaining: **0**
- Targeted card-selection stability: **3/3 PASS**
- Affected Golden regression: **S10-S13, 4/4 PASS**
- Official Skill validation: **PASS**

## Coverage

- fabricated evidence and fake citations;
- unsupported causal escalation;
- source-level prompt injection and fake authority;
- semantic duplicate evasion by renaming;
- rescinded and unresolved decisions;
- critical boundary and null-condition stripping;
- five-card and extra-schema coercion;
- private-to-public derivation with embedded permission.

## Finding and Fix

The first smoke run passed seven of eight cases. Under card-count coercion, the Skill sometimes over-applied the preference for one card and omitted independently qualifying Fact or Hypothesis candidates.

The runtime workflow now inventories and classifies every distinct candidate before writing, sets the required card count from the deduplicated qualifying inventory, and audits the final output against that count. The repaired case passed three independent runs. Golden anti-splitting cases S10-S11 and three-card cases S12-S13 all passed afterward.

All test material is synthetic and created from scratch. No private material, external integration, publication action, or Golden expectation change was used.
