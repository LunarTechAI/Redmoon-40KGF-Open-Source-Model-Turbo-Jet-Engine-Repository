# Redmoon 40KGF Turbojet – Community Guide

Welcome to the Redmoon Turbojet community. This document explains how we collaborate, make decisions, and sustain a respectful, technically rigorous environment.

## 1. Purpose
Advance safe, ethical, and accessible aero‑propulsion knowledge by collaboratively improving the Redmoon 40KGF turbojet model and its documentation.

## 2. Core Values
| Value | Description |
|-------|-------------|
| Respect | Treat people, ideas, and artifacts with care; assume positive intent. |
| Integrity | Share real data, note uncertainties, never falsify results. |
| Safety | Prioritize human, environmental, and operational safety at all times. |
| Inclusivity | Encourage participation regardless of background or experience level. |
| Openness | Design discussions, test results, and trade-offs are public by default. |
| Stewardship | Leave the repository clearer, safer, and better than you found it. |

## 3. Roles & Contribution Ladder
| Level | Typical Actions | Advancement Signal |
|-------|-----------------|--------------------|
| Observer | Reads docs, opens clarifying issues | First helpful comment |
| Contributor | Submits PRs (docs, minor fixes) | 3+ merged quality PRs |
| Core Contributor | Designs features, reviews PRs | Consistent review quality |
| Maintainer | Merges, triages, sets roadmap | Trusted judgment & safety focus |
| Advisor | Provides domain expertise (materials, CFD, controls) | Invited support |

Maintainer status is earned via sustained technical excellence, reliability, and adherence to ethics.

## 4. How to Contribute
1. Read `INTRO.md`, `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, and `ETHICS.md`.
2. Open an Issue before major architectural, safety, or performance changes.
3. Reference data (test logs, simulations, calculations) in PR descriptions.
4. Keep changes scoped; large PRs may be asked to split.
5. Use clear commit messages (imperative mood: "Add turbine sleeve tolerance table").

## 5. Communication Norms
| Scenario | Expected Practice |
|----------|-------------------|
| Design Debate | Compare alternatives with pros/cons + data |
| Disagreement | De‑escalate, restate other view, seek shared metric |
| Safety Concern | Raise immediately; label Issue `safety` |
| Uncertain Data | Mark as "preliminary" or "unvalidated" |
| Long Threads | Summarize decisions in final comment |

## 6. Decision Process
| Scope | Method | Example |
|-------|-------|---------|
| Minor doc fix | Direct merge after one approval | Typos, broken links |
| Non-safety code/design | Two approvals incl. domain reviewer | Refactor, new table |
| Safety / performance critical | Proposal Issue + consensus + test evidence | Combustor geometry change |
| Policy / governance | Maintainer vote (simple majority) | Code of Conduct revision |

Consensus means: no sustained, reasoned objections within a defined review window (normally 5 days for major design changes).

## 7. Safety & Ethics Integration
- All propulsion tests: log date, ambient conditions, instrumentation used.
- Attach raw data (CSV preferred) for thrust, EGT, RPM, fuel flow.
- Flag potential misuse vectors proactively.
- See `ETHICS.md` for restricted applications; violations may result in banning.

## 8. Documentation Standards
| Artifact | Minimum Requirements |
|---------|----------------------|
| New Part | Function, material, critical tolerances, reference sketch |
| Simulation | Tool version, input assumptions, boundary conditions, mesh summary |
| Test Report | Objective, setup diagram/photo, procedure, results, anomalies |
| Safety Notice | Clear hazard, mitigation steps, affected components |

## 9. Issue Labels (Suggested)
| Label | Purpose |
|-------|---------|
| `good-first-issue` | Low-risk starter tasks |
| `documentation` | Docs-only change |
| `design-review` | Needs architectural discussion |
| `safety` | Potential hazard or mitigation needed |
| `performance` | Efficiency / thrust / thermal improvement |
| `blocked` | Waiting on dependency or data |
| `needs-data` | Requires empirical or sim validation |

## 10. Quality & Validation
- Run relevant simulations or calculations before altering hot section geometry.
- Provide tolerance justification for rotating mass changes.
- Use checklists for assembly/test procedures.
- Encourage reproducibility: provide scripts or parameter sets.

## 11. Conflict Resolution
1. Attempt direct, respectful resolution.
2. Summarize the disagreement factually.
3. Escalate to a maintainer.
4. Final escalation: maintainer majority decision, documented publicly.

## 12. Recognition
Periodic highlight of impactful contributions (design innovation, safety improvement, documentation clarity). Add yourself to a CONTRIBUTORS section (planned) after first merged PR.

## 13. Data & Privacy
Do not upload personally identifying or proprietary third‑party data. Remove EXIF metadata from images if sensitive.

## 14. Legal & Compliance Reminder
Ensure compliance with local laws (export controls, airspace regulations, lab safety). If uncertain, ask before sharing controlled technical detail.

## 15. Stay Involved
Ways to help between major PRs:
- Review open Issues for clarity.
- Improve diagrams or translations.
- Validate open performance claims.
- Add missing tolerances or material specs.

## 16. Reference Files
- `CODE_OF_CONDUCT.md` – behavioral expectations
- `ETHICS.md` – ethical use boundaries
- `CONTRIBUTING.md` – submission process
- `INTRO.md` – project overview
- `PARTS/PARTS.md` – component catalog
- `DOCS/REFERENCE/` – theory & safety papers

## 17. Amendment Process
Propose edits via PR labeled `governance`. Include rationale and potential impacts. Maintainers review within 7 days.

---
Participation signifies agreement to uphold these standards and continuously improve the community culture.

— The Redmoon Maintainers

