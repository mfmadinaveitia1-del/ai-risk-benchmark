# Fuselage Join Twin

A browser simulation of a robotic fuselage join cell for an A320-family aircraft (section 15/21 orbital and longitudinal riveting). It shows how **multi-agent systems, digital twins, edge AI and IoT** work together in an *industrial metaverse* view, in the spirit of Siemens Xcelerator / Tecnomatix Process Simulate and Industrial Edge.

> Concept demo with simulated data. Not an Airbus or Siemens product, and not based on real production data.

**Live demo:** https://mfmadinaveitia1-del.github.io/ai-risk-benchmark/fuselage-join-twin/ (once GitHub Pages is on for this repo)

## What it shows

- **Dashboard objective:** one shared live view for shift lead, engineering, quality and maintenance. The goals are to deliver on takt, allow zero quality escapes and surface risks before they stop the line.
- **Data path:** IoT sensors → Edge AI → Digital twin → Agents → People, with commands fed back to the robots.
- **Isometric cell:** 6 riveting robots on LH/RH rails, a vision gantry, 2 AGVs and 176 fasteners. You can switch between three layers: Physical, Digital twin and Industrial metaverse.
- **11 agents:** a cell supervisor, 6 robot agents, QA vision, logistics, predictive maintenance and twin sync. The agents trade work between each other, order parts and pause robots.
- **Scripted scenario:** a spindle bearing fault on R3 at T+16 s. The edge anomaly model flags it, R3 hands over its queue, the twin checks the new plan for collisions (virtual commissioning), an AGV brings a spare spindle and R3 rejoins. You can also inject faults and QA defects yourself.
- **Live KRIs and KPIs:** each indicator has thresholds, a status and its data path.
  - **KRIs:** spindle health, edge latency, twin deviation, inspection backlog, fastener supply, schedule risk, open rework.
  - **KPIs:** OEE, first-pass yield, availability, fastener rate, re-plan time.

## Run locally

It is a single self-contained `index.html` with no build step. Open it in a browser.

## Tech

Vanilla JavaScript and Canvas 2D (isometric projection, 2-link inverse kinematics for the arms), CSS grid, Google Fonts.

## Author

Miguel Figueroa, engineer and project manager, Hamburg.
