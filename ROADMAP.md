# Project Roadmap – Redmoon 40KGF Turbojet

This roadmap lays out the structured path from the current repository state (sketches, preliminary parts list, governance docs) to a fully documented, reproducible, safely testable turbine platform including mechanical CAD, firmware, ECU/ESU electronics, manufacturing instructions, validation data, and educational materials.

---
## 0. Current Status (Baseline)
| Domain | Status | Gaps |
|--------|--------|------|
| Sketches / Concept Imagery | ✅ Rich set in `DOCS/SKETCHES/` | Need dimensioned & toleranced CAD |
| Parts Catalog | ✅ `PARTS.md` functional descriptions | Missing BOM with qty, sourcing, cost |
| Manuals / Reference | Partial PDFs in `DOCS/REFERENCE/` | No unified build + test manual |
| Governance & Ethics | ✅ (Code of Conduct, Ethics, Contributing, Community) | Periodic review cadence not formalized |
| CAD Models | ❌ Not yet committed | Require parametric source + neutral exports |
| Firmware / ECU | ❌ Absent | Architecture, requirements, safety interlocks |
| Electronics (ESU/Control) | ❌ Not defined | Schematics, PCB, harness map |
| Test Data | ❌ None | Need validation framework & data format |
| Safety Protocol | Partial reference PDF | Formal hazard analysis & test checklist |
| Simulation (CFD/FEA) | ❌ None public | Need baseline aerodynamic & thermal models |
| Assembly Procedures | ❌ None | Step-by-step with torque specs & QA points |
| Compliance | ❌ Not addressed | Regulatory guidance (local airspace, noise) |

---
## 1. Guiding Principles
1. Safety before performance
2. Reproducibility before optimization
3. Transparency over proprietary shortcuts
4. Incremental validation (bench → subsystem → integrated engine)
5. Ethical boundary enforcement (see `ETHICS.md`)

---
## 2. Workstreams
| Code | Workstream | Objective |
|------|------------|-----------|
| WS0 | Parts Inventory & Completeness Audit | Establish authoritative baseline list (all parts, status, ownership, missing data) before design formalization |
| WS1 | Mechanical CAD & Drawings | Fully dimensioned, toleranced 3D models + 2D manufacture drawings |
| WS2 | Combustion & Thermal Analysis | Flame stability, pattern factor, material temperature margins |
| WS3 | Rotor Dynamics & Bearings | Critical speed map, balancing procedure, bearing selection & lubrication |
| WS4 | Electronics / ECU / ESU | Control logic, safety interlocks, PCB + firmware stack |
| WS5 | Instrumentation & Telemetry | Sensor suite, logging format, data integrity pipeline |
| WS6 | Manufacturing & Assembly | Fabrication methods, jigs, step-by-step assembly & QA |
| WS7 | Test & Validation | Structured test plans (cold spin, ignition, throttle ramps) |
| WS8 | Safety & Compliance | Hazard analysis (FMEA), risk controls, regulatory notes |
| WS9 | Documentation & Education | Manuals, tutorials, diagrams, glossary, onboarding |
| WS10 | Community & Governance | Review cadence, contributor recognition, policy evolution |

---
## 3. Phased Milestones

### Phase 0 – Parts Completeness & Baseline Audit
Purpose: Ensure every referenced or implied component is enumerated with minimal metadata before CAD & analysis investments.
Deliverables:
- Master Parts Register (MPR) with fields: Part ID, Name, Subsystem, Rev, Source (make/buy), Status (sketch/CAD/mfg), Material (planned), Critical? (Y/N), Owner.
- Gap Report: list of parts mentioned in docs but absent from register.
- Initial sourcing notes for COTS (bearings, sensors, fasteners, electronics).
- Draft numbering scheme (e.g., RM-XX-YYY where XX=subsystem code).
- Ownership matrix assigning provisional maintainers.
Exit Criteria:
- 100% of parts in `PARTS.md`, `SKETCHES.md`, reference PDFs mapped to register entries.
- ≤5% entries with unknown material or status (flagged for Phase 1 resolution).
- Version-controlled register committed (CSV + Markdown summary).
- Issue tags created for missing data (`parts-metadata`).


### Phase 1 – CAD Foundation
Deliverables:
- Parametric CAD for: inlet runner, combustor shell, NGV, turbine sleeve, cartridge receiver, transit ring
- 2D drawings (PDF + DXF) with: material, finish, tolerances, rev tag
- Initial BOM (rev A) with indicative suppliers & rough cost
- CAD contribution guidelines (`/Redmoon-40KGF-MODEL/CAD/CAD.md` expansion)
Exit Criteria:
- 100% of currently sketched parts have CAD + neutral format (STEP)
- BOM coverage ≥ 80% of assemblies

### Phase 2 – Analytical Backbone
Deliverables:
- CFD baseline: inlet → combustor mass flow distribution (mesh + report)
- Thermal calc: NGV metal temp estimate vs allowable
- Rotor dynamics spreadsheet: critical speed vs operating envelope
- Material selection matrix (hot vs cold section)
Exit Criteria:
- Documented assumptions + sensitivity notes
- Pattern factor preliminary target defined

### Phase 3 – Firmware & Electronics Architecture
Deliverables:
- ECU functional requirements (auto-start sequence, fault states, logging)
- ESU (Engine Support Unit) / control board block diagram
- Draft schematics + PCB layout (rev A) + BOM (electronics)
- Firmware repo structure (boot, control loop, sensor drivers, comms)
Exit Criteria:
- Simulated control loop timing budget
- Safety interlock list (overspeed, overtemp, flameout detection)

### Phase 4 – Manufacturing & Assembly Protocol
Deliverables:
- Machining guidance (tooling notes, preferred processes)
- Assembly checklist with torque specs & inspection points
- Balancing procedure (static + dynamic) for rotating group
- Lubrication / fuel system plumbing diagrams
Exit Criteria:
- Dry build achievable without ambiguity
- QA checklist v1 published

### Phase 5 – Bench Testing & Validation
Deliverables:
- Test cell layout & safety perimeter diagram
- Instrumentation plan (sensor list + calibration sheet)
- Test sequence scripts: cold spin, ignition, idle stabilization, throttle ramp, endurance
- Data schema (CSV columns: timestamp, RPM, EGT, thrust, fuel_flow, ambient_T, ambient_P)
- Initial performance dataset + analysis notebook
Exit Criteria:
- Stable idle & controlled acceleration without surge
- Data reproducibility across ≥2 runs

### Phase 6 – Iterative Optimization
Deliverables:
- Combustor revision (if required) for improved pattern factor
- Inlet or NGV geometry tweaks with CFD deltas
- ECU firmware refinement (PID gain tuning, anomaly recovery logic)
- Efficiency summary vs baseline
Exit Criteria:
- Documented performance improvement (e.g., SFC reduction or thermal margin increase)

### Phase 7 – Educational & Outreach Package
Deliverables:
- Illustrated end-to-end build guide (PDF + web markdown)
- Curriculum module (lesson objectives, lab exercises)
- Annotated exploded diagram poster
- Glossary of terms & symbols
Exit Criteria:
- External reviewer (non-core) can navigate build and theory materials

### Phase 8 – Stabilization & Release Candidate
Deliverables:
- Tagged release (v1.0.0) with checksum manifest
- Consolidated LICENSE clarifications (software vs hardware artifacts)
- Final hazard + mitigation matrix
Exit Criteria:
- No open critical Issues (safety/performance blocking)
- Sign-off from ≥2 maintainers across mechanical + firmware + safety domains

### Phase 9 – Post-Release Governance
Deliverables:
- Maintenance schedule (cadence for dependency / doc review)
- Roadmap update process (quarterly re-baseline)
- Contribution metrics dashboard plan
Exit Criteria:
- Governance PR merged updating `COMMUNITY.md`

---
## 4. Detailed Deliverable Matrix
| Workstream | Key Artifacts | Format | Acceptance Gate |
|------------|--------------|--------|-----------------|
| WS1 | CAD models + 2D drawings | STEP, SLDPRT, PDF | Peer mech review + tolerance sanity |
| WS2 | CFD & thermal reports | Markdown + images | Assumption transparency + mesh independence note |
| WS3 | Rotor dynamics sheet | Spreadsheet (CSV/ODS) | Critical speeds outside operating band |
| WS4 | ECU architecture & firmware skeleton | Markdown + source tree | Builds + passes lint/static checks |
| WS4 | PCB schematic & layout | KiCad source + PDF | ERC/DRC clean + BOM export |
| WS5 | Telemetry schema | JSON/Markdown | Column definitions & units validated |
| WS6 | Assembly guide | Markdown + photos | Dry run by non-author reviewer |
| WS7 | Test logs & analysis | CSV + notebook | Reproducibility across runs |
| WS8 | FMEA & safety checklist | Spreadsheet + Markdown | Mitigations mapped to risks |
| WS9 | Education pack | PDF + MD | External learner comprehension feedback |
| WS10 | Governance updates | MD | Maintainer vote recorded |

---
## 5. Backlog (Not Yet Scheduled)
- Add multi-fuel capability (kerosene / sustainable aviation fuel blend study)
- Add thrust vectoring nozzle concept study
- Modular afterburner research (ethics & safety gated)
- Noise attenuation shroud design
- Emissions characterization rig integration
- Digital twin (simulation + live data calibration)

---
## 6. Risk Register (Initial)
| Risk | Impact | Likelihood | Mitigation |
|------|--------|-----------|------------|
| Incomplete CAD tolerances | Mis-machined parts | Medium | Early tolerance review checklist |
| Rotor imbalance | Bearing failure / hazard | Medium | Balancing protocol + trial weights |
| Combustion instability | Hot spots / turbine damage | Medium | Staged testing + EGT array (future) |
| Firmware fault (overspeed) | Catastrophic failure | Low | Dual-threshold overspeed + hardware cutoff |
| Data inconsistency | Misleading performance claims | Medium | Standard schema + validation script |
| Ethical misuse | Reputational & legal risk | Low | Clear ETHICS + reporting channel |

---
## 7. Success Metrics (v1.0)
| Metric | Target |
|--------|--------|
| Stable idle RPM variance | < ±3% over 5 min |
| Throttle response (idle→75%) | < 4 s without surge |
| Pattern factor (turbine inlet) | < ±80 °C (est. or measured) |
| Specific fuel consumption (baseline) | Documented ± accuracy band |
| Documentation completeness (review checklist) | ≥ 95% items checked |
| Safety incidents during test phase | 0 recordable injuries |

---
## 8. Issue & Milestone Tagging Convention
| Tag | Meaning |
|-----|---------|
| `phase0-parts` | Items required for Phase 0 exit |
| `phase1-cad` | Items required for Phase 1 exit |
| `phase2-analysis` | Analytical tasks for Phase 2 |
| `safety` | Impacts operational safety |
| `firmware` | ECU / embedded work |
| `electronics` | PCB / hardware control |
| `education` | Docs & learning artifacts |
| `governance` | Policy & community updates |

Milestones: `P1-CAD`, `P2-Analysis`, `P3-Firmware`, ..., `P8-Release`, `P9-Governance`.

---
## 9. Contribution On-Ramp
| Skill Level | Suggested First Tasks |
|-------------|----------------------|
| Beginner | Tidy documentation, glossary additions, minor drawing annotations |
| Intermediate | CFD mesh validation, schema script, assembly photo doc |
| Advanced | Combustor optimization, rotor dynamics calc, ECU safety state machine |

---
## 10. Review Cadence
| Cadence | Activity |
|---------|---------|
| Weekly | Standup Issue summary (open PRs, blockers) |
| Biweekly | Phase progress checkpoint |
| Monthly | Risk register update & metric review |
| Quarterly | Roadmap re-baseline & backlog grooming |

---
## 11. Change Management
- Significant roadmap edits require PR tagged `governance` + maintainer majority.
- Phase completion announced via release notes entry.
- Archive superseded analysis in `DOCS/ARCHIVE/` (planned) with rev tags.

---
## 12. End-State Definition (v1.0.0)
Repository contains:
- Complete mechanical CAD (parametric + neutral)
- Fully documented BOM (cost, supplier, material spec)
- ECU firmware (auto-start, telemetry, safety interlocks) + ESU electronics design
- Manufacturing + assembly manual (step, torque, inspection)
- Test & validation dataset with analysis notebooks
- Safety protocol & FMEA
- Educational pack & glossary
- Governance + ethics documents maintained
All validated via reproducible build & bench run logs.

---
## 13. Post v1.0 Vision
- v1.1: Efficiency improvements (inlet / combustor rev), additional sensors
- v1.2: Expanded fuel compatibility + emissions baseline
- v2.0: Optional vectoring / modular expansion platform (ethics-gated)

---
For clarifications or roadmap proposals, open an Issue labeled `roadmap` or reach out via `CONTACTS.md`.

— The Redmoon Maintainers

