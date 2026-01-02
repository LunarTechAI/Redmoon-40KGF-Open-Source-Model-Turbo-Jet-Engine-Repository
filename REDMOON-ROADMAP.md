# Redmoon Turbojet Engine Family — Strategic Roadmap

**Version:** 1.0  
**Last Updated:** December 30, 2024  
**Classification:** Public — Community Initiative

---

## Vision Statement

Redmoon aims to become the world's leading platform for accessible aerospace propulsion technology, spanning a complete family of turbojet engines from 10KGF to 500KGF, supported by a comprehensive knowledge library and AI-powered development tools.

---

## Table of Contents

1. [Engine Family Portfolio](#1-engine-family-portfolio)
2. [Knowledge Library & Documentation](#2-knowledge-library--documentation)
3. [AI Agents & Development Tools](#3-ai-agents--development-tools)
4. [Development Phases](#4-development-phases)
5. [Success Metrics](#5-success-metrics)

---

## 1. Engine Family Portfolio

### 1.1 Complete Engine Range

The Redmoon family will span eight thrust classes to address all market segments:

| Model | Thrust | Target Applications | Status | Timeline |
|-------|--------|---------------------|--------|----------|
| **Redmoon 10KGF** | 10 kg (22 lbf) | Small RC jets, STEM education, research testbeds | 🔴 Planned | Q2 2025 |
| **Redmoon 20KGF** | 20 kg (44 lbf) | Medium RC jets, light UAV propulsion, training platforms | 🔴 Planned | Q2 2025 |
| **Redmoon 40KGF** | 40 kg (88 lbf) | Heavy-lift UAVs, experimental aviation, research | 🟡 In Development | Q1 2025 |
| **Redmoon 80KGF** | 80 kg (176 lbf) | Large cargo drones, tactical UAVs, sport jets | 🔴 Planned | Q3 2025 |
| **Redmoon 100KGF** | 100 kg (220 lbf) | Commercial cargo drones, military UAVs, personal aircraft | 🔴 Planned | Q3 2025 |
| **Redmoon 150KGF** | 150 kg (330 lbf) | Heavy cargo logistics, ISR platforms, experimental jets | 🔴 Planned | Q4 2025 |
| **Redmoon 200KGF** | 200 kg (440 lbf) | Large UAV systems, light manned aircraft, multi-engine configs | 🔴 Planned | Q4 2025 |
| **Redmoon 500KGF** | 500 kg (1,102 lbf) | Manned aircraft, heavy-lift platforms, aerospace propulsion R&D | 🔴 Planned | Q4 2025 |

### 1.2 Engine Class Specifications (Preliminary)

#### Micro Class (10–20 KGF)
- **Target Weight:** 1.5–3 kg
- **Fuel Consumption:** 0.2–0.5 kg/min
- **Applications:** Education, hobby RC, micro-UAV
- **Key Features:** Low cost, easy maintenance, starter-friendly

#### Standard Class (40–100 KGF)
- **Target Weight:** 4–10 kg
- **Fuel Consumption:** 0.8–2.5 kg/min
- **Applications:** Commercial drones, experimental aircraft, defense
- **Key Features:** Balanced performance, modular ECU, multi-fuel capability

#### Heavy Class (150–500 KGF)
- **Target Weight:** 15–50 kg
- **Fuel Consumption:** 3–12 kg/min
- **Applications:** Manned aircraft, heavy logistics, military platforms
- **Key Features:** High reliability, redundant systems, advanced cooling

### 1.3 Modular Architecture Benefits

All engines will share:
- **Common ECU Platform:** Scalable firmware across thrust classes
- **Standardized Interfaces:** Fuel, electrical, mounting compatibility
- **Shared Component Families:** Bearings, seals, sensors
- **Unified Documentation:** Consistent technical approach

---

## 2. Knowledge Library & Documentation

### 2.1 Library Structure

```
LIBRARY/
├── MODELS/
│   ├── CAD/                    # Parametric models (STEP, SLDPRT, Fusion)
│   ├── CFD/                    # Flow simulation models
│   ├── FEA/                    # Structural analysis models
│   └── DIGITAL-TWIN/           # Real-time simulation models
│
├── RESEARCH-PAPERS/
│   ├── COMBUSTION/             # Flame stability, efficiency
│   ├── AERODYNAMICS/           # Compressor, turbine design
│   ├── MATERIALS/              # High-temp alloys, coatings
│   ├── CONTROLS/               # ECU algorithms, safety systems
│   └── APPLICATIONS/           # UAV integration, case studies
│
├── BOOKS/
│   ├── FUNDAMENTALS/           # Gas turbine theory
│   ├── DESIGN-GUIDES/          # Practical engineering
│   ├── SAFETY-MANUALS/         # Operations, protocols
│   └── EDUCATIONAL/            # STEM curriculum materials
│
├── COURSES/
│   ├── PROPULSION-101/         # Introduction to jet propulsion
│   ├── THERMODYNAMICS/         # Brayton cycle, heat transfer
│   ├── AERODYNAMICS/           # Compressor & turbine design
│   ├── COMBUSTION/             # Combustor design & analysis
│   ├── MATERIALS-SCIENCE/      # High-temp materials, coatings
│   ├── CONTROL-SYSTEMS/        # ECU design, firmware, safety
│   ├── MANUFACTURING/          # CNC, casting, assembly
│   ├── TESTING-VALIDATION/     # Test protocols, instrumentation
│   └── CERTIFICATION/          # Regulatory compliance, airworthiness
│
└── TRANSLATIONS/
    ├── EN/                     # English (primary)
    ├── ES/                     # Spanish
    ├── FR/                     # French
    ├── DE/                     # German
    ├── ZH/                     # Chinese (Simplified)
    ├── JA/                     # Japanese
    ├── KO/                     # Korean
    ├── RU/                     # Russian
    ├── AR/                     # Arabic
    ├── PT/                     # Portuguese
    ├── HI/                     # Hindi
    ├── NL/                     # Dutch
    └── IT/                     # Italian
```

### 2.2 Engineering Courses

Comprehensive engineering courses spanning turbojet, turbofan, and military afterburning engine technology:

#### Foundational Courses

| Course | Level | Duration | Format | Timeline |
|--------|-------|----------|--------|----------|
| **ENG-101: Gas Turbine Fundamentals** | Beginner | 10 hours | Video + Labs | Q1 2025 |
| **THERMO-201: Thermodynamics for Propulsion** | Intermediate | 16 hours | Video + Exercises | Q1 2025 |
| **AERO-201: Compressor & Turbine Aerodynamics** | Intermediate | 20 hours | Video + CFD Labs | Q1 2025 |
| **COMB-201: Combustion Engineering** | Intermediate | 16 hours | Video + Simulation | Q2 2025 |
| **MAT-201: High-Temperature Materials** | Intermediate | 12 hours | Video + Case Studies | Q2 2025 |

#### Turbojet Engine Specialization

| Course | Level | Duration | Focus Areas | Timeline |
|--------|-------|----------|-------------|----------|
| **TJ-301: Turbojet Engine Design** | Advanced | 24 hours | Axial compressor, annular combustor, axial turbine | Q2 2025 |
| **TJ-302: Turbojet Performance Analysis** | Advanced | 16 hours | Thrust equations, SFC, operating maps | Q2 2025 |
| **TJ-303: Small Turbojet Engineering** | Advanced | 20 hours | Micro-turbines, RC jets, UAV propulsion | Q2 2025 |
| **TJ-304: Turbojet ECU & Controls** | Advanced | 24 hours | FADEC, fuel scheduling, safety systems | Q3 2025 |
| **TJ-305: Turbojet Manufacturing** | Advanced | 20 hours | Precision machining, blade casting, assembly | Q3 2025 |

#### Turbofan Engine Specialization

| Course | Level | Duration | Focus Areas | Timeline |
|--------|-------|----------|-------------|----------|
| **TF-301: Turbofan Engine Architecture** | Advanced | 24 hours | Bypass ratio, fan design, nacelle integration | Q2 2025 |
| **TF-302: High-Bypass Turbofans** | Advanced | 20 hours | Commercial aviation, CFM56, GE90 architecture | Q3 2025 |
| **TF-303: Low-Bypass Turbofans** | Advanced | 20 hours | Military applications, mixed exhaust, vectoring | Q3 2025 |
| **TF-304: Turbofan Performance Optimization** | Expert | 16 hours | Cycle analysis, efficiency trades, noise reduction | Q3 2025 |
| **TF-305: Geared Turbofan Technology** | Expert | 12 hours | PW GTF architecture, gear systems, future trends | Q4 2025 |

#### Military Afterburning Engine Specialization (F-16 F110/F100 Class)

| Course | Level | Duration | Focus Areas | Timeline |
|--------|-------|----------|-------------|----------|
| **MIL-401: Afterburning Turbofan Fundamentals** | Expert | 24 hours | Augmentor design, fuel injection, flame holders | Q3 2025 |
| **MIL-402: F100/F110 Engine Architecture** | Expert | 32 hours | P&W F100, GE F110 deep dive, design philosophy | Q3 2025 |
| **MIL-403: Variable Geometry Systems** | Expert | 20 hours | Variable inlet, nozzle, bypass, stator scheduling | Q4 2025 |
| **MIL-404: Military Engine Controls** | Expert | 24 hours | DEEC, thrust management, envelope protection | Q4 2025 |
| **MIL-405: Supersonic Propulsion** | Expert | 20 hours | Inlet design, afterburner modes, nozzle matching | Q4 2025 |
| **MIL-406: Fighter Engine Maintenance** | Expert | 16 hours | LRU replacement, IETM, condition monitoring | Q4 2025 |

#### Capstone & Certification

| Course | Level | Duration | Focus Areas | Timeline |
|--------|-------|----------|-------------|----------|
| **CAP-501: Engine Design Project** | Master | 40 hours | Full engine preliminary design | Q4 2025 |
| **CAP-502: Test Cell Operations** | Master | 24 hours | Instrumentation, test procedures, data analysis | Q4 2025 |
| **CERT-501: Certification & Airworthiness** | Master | 16 hours | FAA/EASA, type certification, continued airworthiness | Q4 2025 |

**Course Features:**
- 📹 **Video Lectures** — Professional instruction from aerospace engineers
- 🧪 **Hands-on Labs** — Practical exercises with real engine data
- 📊 **Simulation Projects** — CFD, thermodynamic cycle, control system modeling
- 🔧 **Hardware Sessions** — Disassembly/assembly of actual engine components
- 📝 **Assessments** — Quizzes, projects, practical exams
- 🌍 **Multi-language** — Available in 13+ languages
- 🤖 **AI Tutoring** — Powered by Redmoon Support Agent

**Certification Tracks:**

| Track | Courses Required | Hours | Certification |
|-------|------------------|-------|---------------|
| **Propulsion Fundamentals** | ENG-101, THERMO-201, AERO-201 | 46h | Redmoon Associate |
| **Turbojet Specialist** | + TJ-301 through TJ-305 | 150h | Redmoon Turbojet Engineer |
| **Turbofan Specialist** | + TF-301 through TF-305 | 138h | Redmoon Turbofan Engineer |
| **Military Propulsion Expert** | + MIL-401 through MIL-406 | 182h | Redmoon Defense Engineer |
| **Master Propulsion Engineer** | All courses + CAP-501, CAP-502, CERT-501 | 300h+ | Redmoon Master |

### 2.3 Documentation Categories

| Category | Description | Formats | Languages |
|----------|-------------|---------|-----------|
| **Technical Manuals** | Build, assembly, maintenance guides | PDF, MD, HTML | 13+ |
| **Safety Protocols** | Operational safety, emergency procedures | PDF, MD | 13+ |
| **Research Papers** | Academic publications, white papers | PDF | English + abstracts |
| **Educational Materials** | Curriculum guides, lab exercises | PDF, PPTX, MD | 13+ |
| **Reference Books** | Foundational texts on turbine technology | PDF | English + select translations |

### 2.4 Translation Pipeline

**Supported Languages (13+):**

| Tier | Languages | Coverage |
|------|-----------|----------|
| **Tier 1 (Full)** | English, Spanish, French, German, Chinese | 100% core documentation |
| **Tier 2 (Core)** | Japanese, Korean, Portuguese, Arabic | 80% core documentation |
| **Tier 3 (Community)** | Russian, Hindi, Dutch, Italian, Turkish, Polish | Community-driven |

**Translation Workflow:**
1. Primary documentation in English
2. AI-assisted translation with human review
3. Community contribution and validation
4. Native speaker technical review

---

## 3. AI Agents & Development Tools

### 3.1 AI Agent Ecosystem

The Redmoon project will integrate AI agents to accelerate development and support the community:

| Agent | Function | Technology | Status |
|-------|----------|------------|--------|
| **Redmoon Design Agent** | CAD generation, parametric optimization, design exploration | Vision + Code AI | 🔴 Planned |
| **Redmoon Analysis Agent** | CFD/FEA pre-processing, result interpretation, optimization suggestions | Scientific Computing AI | 🔴 Planned |
| **Redmoon Documentation Agent** | Auto-documentation, translation, technical writing assistance | LLM + RAG | 🔴 Planned |
| **Redmoon Safety Agent** | Hazard analysis, FMEA assistance, safety protocol generation | LLM + Knowledge Base | 🔴 Planned |
| **Redmoon Support Agent** | Community Q&A, troubleshooting, onboarding | Conversational AI + RAG | 🔴 Planned |
| **Redmoon Code Agent** | Firmware development, ECU programming, simulation scripts | Code Generation AI | 🔴 Planned |

### 3.2 Agent Capabilities

#### Redmoon Design Agent
- **Input:** Requirements (thrust, weight constraints, operating conditions)
- **Output:** Parametric CAD suggestions, component sizing, trade studies
- **Integration:** SolidWorks, Fusion 360, FreeCAD APIs

#### Redmoon Analysis Agent
- **Input:** Geometry, boundary conditions, material properties
- **Output:** Mesh recommendations, solver settings, result summaries
- **Integration:** OpenFOAM, ANSYS Fluent, SimScale

#### Redmoon Documentation Agent
- **Input:** Technical specifications, code comments, meeting notes
- **Output:** Formatted documentation, translations, release notes
- **Integration:** GitHub, GitLab, Confluence

#### Redmoon Safety Agent
- **Input:** Design changes, operational scenarios, incident reports
- **Output:** Risk assessments, mitigation recommendations, safety checklists
- **Integration:** FMEA tools, safety management systems

#### Redmoon Support Agent
- **Input:** User questions, error messages, build logs
- **Output:** Troubleshooting guidance, relevant documentation, escalation
- **Integration:** Discord, Forums, GitHub Issues

#### Redmoon Code Agent
- **Input:** Requirements, existing firmware, hardware specifications
- **Output:** ECU firmware, test scripts, simulation code
- **Integration:** Arduino, STM32, ESP32 toolchains

### 3.3 AI Integration Roadmap

| Phase | Milestone | Timeline |
|-------|-----------|----------|
| **Phase A** | Documentation Agent (translation, formatting) | Q1 2025 |
| **Phase B** | Support Agent (community Q&A) | Q1 2025 |
| **Phase C** | Safety Agent (FMEA assistance) | Q2 2025 |
| **Phase D** | Design Agent (parametric exploration) | Q2 2025 |
| **Phase E** | Analysis Agent (CFD/FEA integration) | Q3 2025 |
| **Phase F** | Code Agent (firmware development) | Q3 2025 |

---

## 4. Development Phases — 2025

### Q1 2025: Foundation
**Focus:** Redmoon 40KGF completion + AI infrastructure

- [ ] Complete 40KGF CAD documentation
- [ ] Finalize ECU firmware architecture
- [ ] Establish manufacturing guidelines
- [ ] Build initial test validation dataset
- [ ] Launch community infrastructure
- [ ] Deploy Documentation Agent
- [ ] Deploy Support Agent

### Q2 2025: Expansion — Micro & Mid Class
**Focus:** 10KGF, 20KGF, Safety & Design AI

- [ ] 10KGF design and prototyping
- [ ] 20KGF design and prototyping
- [ ] Educational curriculum package
- [ ] Multi-language documentation (Tier 1: EN, ES, FR, DE, ZH)
- [ ] Deploy Safety Agent
- [ ] Deploy Design Agent

### Q3 2025: Growth — Standard Class
**Focus:** 80KGF, 100KGF, Analysis & Code AI

- [ ] 80KGF design scaled from 40KGF
- [ ] 100KGF advanced design
- [ ] Commercial partnership program
- [ ] Full research paper library (100+ papers)
- [ ] Deploy Analysis Agent
- [ ] Deploy Code Agent
- [ ] Tier 2 languages (JA, KO, PT, AR)

### Q4 2025: Scale — Heavy Class & Complete
**Focus:** 150KGF, 200KGF, 500KGF, full ecosystem

- [ ] 150KGF heavy-duty design
- [ ] 200KGF advanced configuration
- [ ] 500KGF flagship engine design
- [ ] Complete 8-engine family designs
- [ ] Defense/commercial integrator partnerships
- [ ] Certification pathway documentation
- [ ] Full AI agent ecosystem operational
- [ ] Tier 3 languages (RU, HI, NL, IT)
- [ ] 25+ university partnerships

---

## 5. Success Metrics — End of 2025 Targets

### Engine Development (EOY 2025)

| Metric | Target |
|--------|--------|
| Engines in family | 8 (complete designs) |
| Validated builds | 50+ |
| Test hours logged | 2,500+ |
| Prototype engines running | 4+ (10, 20, 40, 80 KGF) |

### Knowledge Library (EOY 2025)

| Metric | Target |
|--------|--------|
| Research papers | 150+ |
| Books/manuals | 50+ |
| Languages supported | 13 |
| Documentation downloads | 10,000+ |

### AI Agents (EOY 2025)

| Metric | Target |
|--------|--------|
| Agents deployed | 6 (all) |
| Monthly interactions | 25,000+ |
| User satisfaction | 85%+ |
| Tasks automated | 50%+ |

### Community (EOY 2025)

| Metric | Target |
|--------|--------|
| Community members | 5,000+ |
| Active contributors | 100+ |
| University partnerships | 25+ |
| Industry partnerships | 10+ |

---

## Appendix: Engine Family Comparison

```
                    REDMOON TURBOJET ENGINE FAMILY
    ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
    
    THRUST (KGF)     10    20    40    80   100   150   200   500
                     │     │     │     │     │     │     │     │
    ═══════════════════════════════════════════════════════════════
    
    MICRO CLASS      ████  ████                                    
                     │     │                                        
                     │     └── RC Jets, Training                   
                     └── Education, Hobby                          
    
    STANDARD CLASS               ████  ████  ████                  
                                 │     │     │                      
                                 │     │     └── Commercial UAV     
                                 │     └── Tactical UAV             
                                 └── Heavy Lift Drone               
    
    HEAVY CLASS                              ████  ████  ████      
                                             │     │     │          
                                             │     │     └── Manned Aircraft
                                             │     └── Large UAV    
                                             └── Cargo Logistics    
    
    ═══════════════════════════════════════════════════════════════
    PHASE            Q2    Q2    Q1    Q3    Q3    Q4    Q4    Q4
                     2025  2025  2025  2025  2025  2025  2025  2025
    ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

---

*This roadmap is a living document. Updates will be made as development progresses and community input is received.*

— The Redmoon Team
