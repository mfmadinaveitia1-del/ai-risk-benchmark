# A320 FAL Twin

Concept digital twin of an A320 Family final assembly line, rendered as an interactive isometric 3D scene (three.js).

**Goal:** make the final assembly process more efficient by showing where time is lost and testing fixes before they are made on the shop floor.

- Live flow simulation of 8 stations (S50 pre-equip → S41 fuselage join → S40 wing join → S35 systems & cabin → S30 engines → S20 ground tests → paint → flight line)
- Critical path (CPM Gantt) and bottleneck ranking
- Line balancing (Yamazumi) with drag-and-drop work packages
- Quality loop: escaped defects, rework and travelled work
- Improvement levers with a simulated before/after impact report, plus disruption stress tests
- Physical, digital twin and industrial metaverse layers

**Synthetic data:** layout, cycle times, rates, defect rates, costs and station numbers are invented for this concept and do not represent any manufacturer's data.

**Kiosk use:** the page holds a screen wake lock while it is open and visible, so a wall display will not dim or sleep (toggle in the Line pulse panel). If the GPU context is lost it reloads itself.

Open `index.html` in a browser, or view it via GitHub Pages.
