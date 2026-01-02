# Sketches & Component Function Reference

Authoritative visual index of the Redmoon 40KGF turbojet core components. Each sketch below is paired with a concise functional description, design intent notes, and integration context. Use this alongside the parts list in [`Redmoon-40KGF-MODEL/PARTS/PARTS.md`](../../Redmoon-40KGF-MODEL/PARTS/PARTS.md) and fabrication guidance in `MANUAL.md`.

---
## Quick Navigation
- [1. Inlet & Flow Conditioning](#1-inlet--flow-conditioning)
- [2. Combustion System](#2-combustion-system)
- [3. Fuel Evaporation & Mixing](#3-fuel-evaporation--mixing)
- [4. Turbine & Hot Section](#4-turbine--hot-section)
- [5. Bearing & Lubrication Components](#5-bearing--lubrication-components)
- [6. Structural & Retention Hardware](#6-structural--retention-hardware)
- [7. Cowling & External Ducting](#7-cowling--external-ducting)
- [8. Starter & Ancillary Interfaces](#8-starter--ancillary-interfaces)
- [9. Transit / Alignment Rings](#9-transit--alignment-rings)
- [10. Composite View & Assembly Relations](#10-composite-view--assembly-relations)
- [Legend & Design Notes](#legend--design-notes)

### Component Index (Integrated)
Central index tying each image to its functional section. Update this table when adding or revising sketches.

| File | Component / Caption | Section | Core Function (1‑liner) | Rev Status |
|------|---------------------|---------|-------------------------|------------|
| `inlet_runner_sketch.png` | Inlet runner baseline | 1 | Guides ambient air to compressor inducer | Draft |
| `inlet_runner_sketch_airflow.png` | Inlet airflow overlay | 1 | Visualizes boundary layer & pathlines | Draft |
| `inlet_runner_sketch_top_down.png` | Inlet top-down geometry | 1 | Shows concentric datum & symmetry | Draft |
| `combustion_chamber_sketch.png` | Combustor shell & hole pattern | 2 | Primary/secondary/dilution staging | Draft |
| `combustion_chamber_out_sketch.png` | Combustor outlet zone | 2 | Dilution / pattern factor conditioning | Draft |
| `evaporator_sketch.png` | Fuel evaporator | 3 | Pre-vaporizes fuel before flame zone | Draft |
| `ngv_evaporator_sketch_no_dimensions.png` | NGV + evaporator relation | 3/4 | Spatial fuel path clearance to NGV | Draft |
| `ngv_with_protecting_layer_sketch.png` | NGV w/ shielding layer | 4 | Directs flow & manages metal temperature | Draft |
| `turbine_shaft_sleeve_sketch.png` | Turbine shaft sleeve | 4 | Couples wheel + isolates heat | Draft |
| `turbocharger_billetwheel_turbineshaft_turbinewheelsketch.png` | Rotor composite | 4 | Energy extraction & rotor dynamics base | Draft |
| `oil_ring_sketch.png` | Oil ring | 5 | Lubricant metering / slinging | Draft |
| `bearing_pad_component_engineering_sketch.png` | Bearing pad | 5 | Distributes bearing/thrust loads | Draft |
| `cartridge_receiver_sketch_refined_holes.png` | Cartridge receiver | 6 | Locates core & fastener indexing | Draft |
| `cowling_sketch.png` | Cowling shell | 7 | External enclosure & intake shaping | Draft |
| `cowling_engineering_sketch_airflow.png` | Cowling airflow view | 7 | Highlights pressure recovery zones | Draft |
| `starter_connector_sketch.png` | Starter connector | 8 | Transmits start torque | Draft |
| `transit_ring_sketch.png` | Transit ring (initial) | 9 | Spacing & handling protection | Draft |
| `transit_ring_sketch_refined.png` | Transit ring refined | 9 | Weight & alignment optimization | Draft |
| `transit_ring_engineering_sketch.png` | Transit ring engineering | 9 | Finalized hole pattern & tolerances | Draft |

Legend: Rev Status placeholders (Draft / Rev A / Rev B). Promote after validation or dimensional release.

---
## 1. Inlet & Flow Conditioning
Efficient, uniform, swirl‑minimal airflow into the compressor/turbocharger core is critical for surge margin and combustion stability.

### Inlet Runner Series
![Inlet Runner Sketch](inlet_runner_sketch.png)
![Inlet Runner Sketch with Airflow](inlet_runner_sketch_airflow.png)
![Inlet Runner Top-Down Sketch](inlet_runner_sketch_top_down.png)
Function: Forms the aerodynamic transition guiding ambient air into the compressor inducer. The airflow overlay highlights expected boundary layer development and core stream contraction. Top‑down geometry indicates alignment datum (X0 plane) used for concentric assembly.
Design Considerations:
- Minimize separation via smooth curvature; avoid sharp area contractions >12% per axial step.
- Surface finish affects inlet pressure recovery; Ra < 3.2 µm preferred.
- Provide drainage or anti-pooling features if fuel mist risk exists during failed start.

---
## 2. Combustion System
Staged air admission + controlled primary zone recirculation ensures stable flame anchoring and turbine inlet temperature distribution.

### Combustion Chamber Core
![Combustion Chamber Sketch](combustion_chamber_sketch.png)
![Combustion Chamber Outlet Sketch](combustion_chamber_out_sketch.png)
Function: Primary confinement of the combusting mixture. The outlet sketch focuses on dilution and temperature conditioning zone before the nozzle guide vanes (NGV). Hole patterns imply staged air: primary (flame stabilization), secondary (completion), dilution (T4 profile shaping).
Design Considerations:
- Maintain equivalence ratio in primary zone ~0.9–1.05 for reliable ignition.
- Dilution hole sizing must achieve <±80°C pattern factor at turbine inlet.
- High-temp alloy (e.g., 310S SS / Inconel 625 for durability); include thermal growth allowance.

---
## 3. Fuel Evaporation & Mixing
Pre-vaporizing fuel improves atomization uniformity and reduces local hotspots.

### Evaporator Assembly
![Evaporator Sketch](evaporator_sketch.png)
Function: Introduces and vaporizes liquid fuel using conduction + convective preheat from compressor discharge air prior to entering flame zone. Reduces droplet size demand on injector.
Notes:
- Control wall film formation; incorporate gentle mixing shear rather than abrupt impingement.
- Stainless or nickel alloy recommended to resist coking.

### NGV & Evaporator Interaction
![NGV and Evaporator Sketch](ngv_evaporator_sketch_no_dimensions.png)
Shows geometric coupling—ensures evaporated fuel path doesn’t impinge directly on first-stage nozzle throats.

---
## 4. Turbine & Hot Section
Extracts energy from expanding combustion gases while controlling swirl and temperature profile.

### Nozzle Guide Vane (NGV)
![NGV with Protecting Layer Sketch](ngv_with_protecting_layer_sketch.png)
Function: Accelerates and directs flow at precise incidence onto turbine wheel. The protecting layer annotation suggests thermal barrier coating or shielding feature for extending substrate life.
Key Parameters:
- Throat area sets mass flow → thrust; maintain machining tolerance ±0.05 mm on chordwise throat gap for repeatability.
- Metal temperature limit guides material (Inconel / Hastelloy).

### Turbine Shaft Sleeve
![Turbine Shaft Sleeve Sketch](turbine_shaft_sleeve_sketch.png)
Function: Couples turbine wheel to rotating shaft; may provide thermal isolation + oil sealing shoulder.
Consider: Interference fit vs. keyed spline; balance correction drill points to be pre‑planned.

### Turbine Wheel / Shaft / Billet Wheel Composite
![Turbocharger Billet Wheel, Turbine Shaft, and Turbine Wheel Sketch](turbocharger_billetwheel_turbineshaft_turbinewheelsketch.png)
Function: Adapted turbocharger core repurposed for axial hot section energy extraction. Ensure rotor critical speed map keeps operating band below 1st bending and above 1st torsional resonances.

---
## 5. Bearing & Lubrication Components
Maintain low-friction, thermally managed rotor support.

### Oil Ring
![Oil Ring Sketch](oil_ring_sketch.png)
Function: Metered distribution of lubricant to journal or thrust interfaces; also serves as a slinger to reduce coking inside hot zones.
Design Notes: Groove geometry influences flow shedding; avoid sharp edges inducing aeration.

### Bearing Pad Component
![Bearing Pad Component Engineering Sketch](bearing_pad_component_engineering_sketch.png)
Function: Local load distribution element—could be part of a thrust or radial bearing support. Chamfers illustrate stress mitigation at fillet transitions.

---
## 6. Structural & Retention Hardware
Provides axial, radial, and thermal growth alignment of stacked modules.

### Cartridge Receiver
![Cartridge Receiver Sketch](cartridge_receiver_sketch_refined_holes.png)
Function: Houses or locates the turbo core / bearing cartridge. Refined hole pattern likely for doweling + fasteners enabling repeatable indexing.
Key Checks:
- Concentricity to inlet runner bore.
- Thermal expansion mismatch vs. cartridge outer diameter.

---
## 7. Cowling & External Ducting
External shell managing intake conditioning, enclosure safety, and airflow visualization.

![Cowling Sketch](cowling_sketch.png)
![Cowling Engineering Sketch with Airflow](cowling_engineering_sketch_airflow.png)
Function: Provides controlled intake capture and optionally supports mounting for accessories. Airflow overlay suggests pressure recovery zones and potential cooling bleed trajectories.
Tip: Smooth internal paint or polish can reclaim fractional percentage in total pressure recovery.

---
## 8. Starter & Ancillary Interfaces
Systems that enable initial rotor spin-up and instrumentation.

### Starter Connector
![Starter Connector Sketch](starter_connector_sketch.png)
Function: Mechanical coupling for external electric or pneumatic starter to transmit torque during spool-up to light-off RPM. Ensure backlash management and disengagement method post self-sustaining speed.

---
## 9. Transit / Alignment Rings
Maintain axial stack, distribute clamping load, assist in shipping/handling.

![Transit Ring Sketch](transit_ring_sketch.png)
![Refined Transit Ring Sketch](transit_ring_sketch_refined.png)
![Transit Ring Engineering Sketch](transit_ring_engineering_sketch.png)
Function: Serves as a structural spacer and/or protective ring during handling. Refinements show hole alignment evolution and potential weight reduction cutouts.
Design Emphasis: Flatness tolerance, parallelism, and surface hardness if used as a thrust reaction surface.

---
## 10. Composite View & Assembly Relations
Some sketches imply relative positioning. Cross-reference rotor stack order: Inlet → Compressor (turbo core) → Diffuser / Evaporator → Combustion Chamber → NGV → Turbine Wheel → Exhaust.

---
## Legend & Design Notes
Terminology & Visual Cues:
- Airflow overlay arrows: primary path vs. dilution or cooling bleeds.
- Highlighted protective layer: thermal barrier or sacrificial shield.
- Refined versions: iteration toward manufacturable tolerances or improved flow distribution.

Recommended Documentation Extensions:
1. Add dimensioned CAD exports (DXF/STEP) to `CAD/` for each part once finalized.
2. Add a revision table (Rev / Date / Change / Author) per component.
3. Introduce simplified FEA snapshots (bearing pad, NGV thermal) to validate assumptions.
4. Include a rotor critical speed plot in a future `ANALYSIS` section.

Manufacturing & Material Quick Hints:
- Hot Section: Nickel alloys (Inconel 625/718) or high-temp stainless; apply solution + age treat where needed.
- Cold Section / Structural: 6061-T6 or 7075-T6 (if isolated from heat) or mild steel for prototypes.
- Fasteners: High-temp stainless (A286) near combustor.
- Surface Prep: Deburr all flow holes; maintain consistent edge radius (0.2–0.4 mm) to reduce stress risers.

Safety & Validation Checklist:
- Leak test fuel path prior to ignition trials.
- Run staged spool tests: (1) dry rotation friction torque, (2) starter engagement, (3) ignition idle stability, (4) transient acceleration.
- Monitor bearing oil outlet temperature ≤ manufacturer spec.

Licensing & Attribution:
All images and descriptive text in this directory are covered by the repository LICENSE. Reuse requires attribution to the Redmoon 40KGF Project.

---
Revision: Enriched functional documentation generated (2025-09-11). Future edits: add dimension tables & performance correlations.

