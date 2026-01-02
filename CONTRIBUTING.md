# Contributing to the Redmoon 40KGF Turbojet

Thank you for your interest in advancing ethical propulsion technology. This guide explains how to propose changes, report issues, share data, and collaborate effectively.

## 1. Read First
Before contributing, familiarize yourself with:
- `INTRO.md` – project overview & goals
- `CODE_OF_CONDUCT.md` – behavioral expectations
- `ETHICS.md` – ethical use boundaries
- `COMMUNITY.md` – collaboration norms & decision process
- `Redmoon-40KGF-MODEL/PARTS/PARTS.md` – component catalog

## 2. Contribution Types
| Type | Examples | Notes |
|------|----------|-------|
| Documentation | Clarifications, diagrams, translations | Must be technically accurate |
| Design Improvements | Geometry refinements, tolerance analysis | Provide rationale & data |
| Safety Enhancements | Guards, failure analysis, risk mitigations | Mark PR with `safety` label |
| Performance Optimization | Combustion efficiency, flow smoothing | Show simulation or test evidence |
| Test Data | Thrust logs, fuel flow, EGT, RPM traces | Include instrumentation & conditions |
| Tooling / Scripts | Analysis utilities, validation scripts | Provide usage instructions |

## 3. Ethical & Legal Constraints
All contributions must comply with local laws, export controls, and the ethical restrictions in `ETHICS.md`. Do not submit controlled technical data or military-specific adaptations.

## 4. Workflow Overview
1. Open an Issue for any non-trivial change (design, structure, safety, performance).
2. Discuss approach; gather consensus if high impact.
3. Fork / branch: `feature/<short-description>` (e.g., `feature/combustor-dilution-v2`).
4. Implement + document.
5. Run checks / provide validation.
6. Open Pull Request (PR) referencing Issue ID.
7. Respond to review feedback promptly.
8. Squash or rebase if requested; maintain clean history.

## 5. Issue Reporting
Include: context, expected vs actual, reproduction steps, environment (tools, materials, test rig), and safety implications if any. Use labels where appropriate (`documentation`, `design-review`, `performance`, `safety`).

## 6. Pull Request Requirements
Each PR should include:
- Clear title (imperative mood)
- Linked Issue (if applicable)
- Summary of change & motivation
- Safety impact (explicitly state "None" if none)
- Validation evidence (simulation screenshots, CSV logs, calculations, photos)
- Backward compatibility notes
- Follow-up tasks (if deferring items)

### Validation Evidence Examples
| Change Type | Evidence |
|-------------|----------|
| Combustor hole pattern | Temperature distribution sim + pattern factor calc |
| Turbine sleeve redesign | Runout measurement & balance analysis |
| Inlet smoothing | CFD pressure recovery vs baseline |
| Oil ring tweak | Oil flow rate before/after and bearing temp trend |

## 7. Coding / Documentation Standards
Even if this repo is design-heavy, keep consistency:
- Use Markdown for documentation; prefer relative paths for linking.
- Keep images in appropriate subdirectories (e.g., `DOCS/SKETCHES/`).
- Use tables for tolerance & parameter summaries.
- Provide units (SI preferred) and define symbols.
- Avoid embedding large binary CAD in PR unless essential—reference external or add compressed neutral formats (STEP, IGES) with justification.

## 8. Data Submission Guidelines
| Field | Requirement |
|-------|------------|
| File Format | CSV or JSON preferred |
| Columns | Include time base, units row or doc section |
| Calibration | Note instrument model & calibration date if possible |
| Ambient Conditions | Pressure, temperature, humidity (if affecting performance) |
| Safety Notes | Any anomalies, excursions, shutdown causes |

## 9. Safety Considerations
Before testing or proposing high-energy modifications:
- Perform risk assessment (rotor containment, fuel handling, hot surfaces)
- Document emergency shutdown method
- NEVER test indoors without proper ventilation and fire mitigation equipment
- Log EGT, fuel flow, and RPM; do not exceed recommended spool thresholds

## 10. Review Expectations
Maintainers and reviewers will look for:
- Technical correctness & clarity
- Evidence-backed claims
- Alignment with ethics & safety
- Minimal scope creep
- Reusability and maintainability

## 11. Large or Breaking Changes
If your change affects multiple subsystems (e.g., combustor architecture, bearing system):
1. Create a design proposal Issue labeled `design-review`.
2. Provide diagrams, calculations, and risk analysis.
3. Allow at least 5 days for community feedback.
4. Incorporate consensus before implementation.

## 12. Attribution & Licensing
By contributing, you affirm you have the right to submit the content and agree it will be released under the project’s LICENSE. Cite third-party references properly. Do not copy proprietary manuals or controlled data.

## 13. Avoiding Common Pitfalls
- Missing units or assumptions in calculations
- Unverified simulation meshes (no mesh independence study)
- Over-claiming performance without test backing
- Large, unfocused PRs mixing unrelated changes

## 14. Continuous Improvement Items (Good First Issues)
- Add missing tolerances to existing part docs
- Translate key docs into additional languages
- Provide structured test data templates
- Create analysis scripts for thrust normalization vs ambient conditions

## 15. Dispute Resolution
If PR feedback feels unclear or conflicting:
1. Summarize concerns factually.
2. Request a maintainer decision.
3. Final decision documented in PR thread.

## 16. Security / Misuse Reporting
Report suspected unethical use or re-hosting for prohibited applications via a confidential Issue or designated contact (see `ETHICS.md`). Provide evidence and context.

## 17. After Your PR is Merged
- Optionally add yourself to CONTRIBUTORS (planned section) with area of focus.
- Help review another open PR to pay it forward.
- Share summarized lessons learned if technical.

## 18. Questions?
Open an Issue labeled `question` or join ongoing design discussions. Polite curiosity is always welcome.

---
Your participation helps make propulsion knowledge safer, more transparent, and more accessible.

— The Redmoon Maintainers

