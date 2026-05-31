# How to Build an OpenLab

A structured guide for building a fully documented multidisciplinary engineering lab, derived from the OpenLab External Epistemic Memory — 257 beliefs extracted from 10+ years of David Malawey's lab development.

---

## 1. Philosophy & Principles

Before purchasing a single tool, internalize these principles. They are what separate a pile of equipment from a functioning lab.

**Mission:** Build the ultimate model lab by openly sharing exact tools, supplies, and methods for everything from traditional fabrication to modern robotics. The focus is hands-on designers and researchers of mechatronics.

**Toyota Methodology:** Five core concepts from Toyota's production system are operationalized (not merely referenced) in the lab:
- **5S** — Sort, Set in order, Shine, Standardize, Sustain
- **Kaizen** — Continuous improvement
- **PDCA** — Plan, Do, Check, Act
- **Yokoten** — Horizontal knowledge sharing
- **Genchi Genbutsu** — Go and see for yourself

**Pull System:** Better to pull a design towards a user application than push a design to fit expected utility. All OpenLab content answers questions that were asked in real life. Don't design for hypothetical uses — wait for a real need to pull the design into existence.

> *Example:* A bit holder was designed to hold tools. During design it was clear it could be configured for drill bits too. But a user informed the designer that tools of many sizes are best accessed in a row, small to large — a grid layout is confusing. The drill bit storage became a completely different design. Only a real user pulling the design produces this insight.

**Standardization Strategy:** Constrain choices deliberately to maximize interoperability and minimize inventory:
- **Fasteners:** M2.5 (small) and M6 (large) as defaults. Stock 30mm and 40mm lengths only — cut 40mm down when 35mm is needed.
- **Wire:** 18 gauge standard for power, 16 gauge for high-current (18V battery) applications.
- **Batteries:** 18650 lithium-ion cells as the standard.
- **Beams:** 3030 aluminum extrusion, DIN rail, EMT conduit, unistrut — no custom structural members.

**Tools vs. Supplies:** Tools are reusable equipment. Supplies are consumable items that pair with tools, parts attainable in bulk, items supporting organization, or items used as consumables. This distinction drives how you organize, inventory, and restock.

**Don't "Worry":** In engineering, "worry" means exerting effort to countermeasure a problem you haven't encountered. Don't add drainage channels before verifying water enters. Prototype without the countermeasure, test in the real environment, then add solutions only for verified issues.

---

## 2. Facility Setup

**Space Reference:** The documented OpenLab occupies approximately 330 square feet (30.5 square meters) with 8-foot (244cm) ceilings, walls and ceiling painted white.

### Lighting
- 5 LED shop lights at 5,000 lumens each — target 1,000 lumens per square meter minimum
- Install **upside-down, oriented at ceiling** to spread light, eliminate bright spots, and reduce harsh shadows
- Pivoting-beam models recommended for adjustable station lighting
- White-painted ceiling and walls enhance distribution
- Links: [Hypertough 7k lumen at Walmart](https://www.walmart.com/ip/Hyper-Tough-7000LM-4Ft-Shop-Light-with-Motion-Sensor-Winged-Day-Light-1PK/1132172978), [JESLED 2-pack on Amazon](https://amzn.to/4cyEC0r)

### Air Filtration
- Honeywell HPA300 and HPA200 HEPA air purifiers, running since 2018
- Low power setting (~40W) runs continuously for gentle air circulation
- Boost to turbo when soldering emits smoke or sanding creates dust — clears room in minutes
- Carbon prefilters changed quarterly, collect VOCs and dust
- Third-party replacement filters available at competitive pricing
- Links: [HPA300](https://amzn.to/4sHtIe3), [HPA200](https://amzn.to/4uo73oC), [filter refills](https://amzn.to/4sHuvf1)

### Environmental Control (Corrosion)
- Hygrometers in sensitive drawers to monitor humidity (room ~50% RH, drawer target ~40%)
- Moisture absorbers: calcium chloride (lasts 6-12 months with 3 tubs per toolbox) or silica gel (reusable, weigh to detect ~20% weight gain)
- Corrosion inhibitor spray (SuperLube 83110) for stored bare steel tools
- Clean rust with BKF (Barkeeper's Friend) and abrasive scrubber
- Links: [Calcium chloride 6-pack $21](https://amzn.to/3GjQ7LK), [Silica bags 100g](https://amzn.to/42jTkmg), [Hygrometer 6-pack](https://amzn.to/40sVaAe), [SuperLube 83110](https://amzn.to/3Iko1B5)

### Wash Station
- Utility sink with hot and cold water
- Reverse osmosis filter (Aquatic Life brand): 3-stage system, fills 5 gallons in ~50 minutes, removes nearly all dissolved solids. Requires continuous water pressure and drain access. ~400 gallon filter life, $15 RO membrane replacement.
- Wall-mounted rack for cleaning substances
- Hanging hooks positioned where items can drip without issues
- Links: [RO filter kit $70](https://amzn.to/3NpbajA), [RO membranes 2-pack $33](https://amzn.to/4rfBWZv), [TDS meter $8](https://amzn.to/4rqBeJc)

---

## 3. Structural Systems

These beam materials and mounting standards form the skeleton of every station, rack, and fixture.

### Beam Material Selection

| Material | Use Case | Strength |
|----------|----------|----------|
| Unistrut/Superstrut | Steel backbone for assemblies requiring rigidity and force | Very high |
| 3030 Aluminum Extrusion | Desk-sized assemblies and machines | High |
| 2020 Aluminum Extrusion | Non-forceful assemblies with accurate datums | Moderate |
| EMT Conduit 3/4in | Long-reaching assemblies, less dimensional accuracy | Moderate |
| EMT Conduit 1/2in | Reach assemblies where datums are less crucial | Moderate |
| Fiberglass 3/8in rod | Tension reinforcement, light torque rotation | Moderate (67kN tensile) |
| 35mm DIN Rail | Modular item mounting with alignment | Low-moderate |

### Sourcing
- **3030 Extrusion:** AutomationDirect preferred — consistent specs, free fast shipping in USA, free custom cut lengths with sub-mm accuracy including 45° angles. [AutomationDirect](https://www.automationdirect.com/adc/shopping/catalog/structural_frames_-z-_rails/t-slotted_rails/30-3030c)
- **DIN Rail:** Steel, 35mm height. [10-pack on Amazon](https://amzn.to/437Bm7Z), [DIN cutter $130](https://amzn.to/47QvuBs)
- **EMT Conduit:** Most affordable steel tube on market. Indexing marks at 1-inch increments. Cut with handheld tube cutter. Soft steel grade — drillable, tappable, paintable, shapeable with carbide burr.

### DIN Rail Accessories
Published 3D-printable brackets on grabCAD:
- DIN-spring (clip-on), tube clamp (round pole), minimal-pi-bracket (15-min Raspberry Pi holder), DIN-rail-pivot (±90° end-to-end), compliant brackets (built-in springs), handy-mount (electrical box)

### Panel Materials
- Expanded PVC (PVC foam): choose 6mm thickness, mark with pencil, cut with utility knife, bond with PVC cement to nearly any material

---

## 4. Toolboxes

The lab is organized into toolboxes (combined storage + workspace), stations (dedicated-activity workstations), and storage (materials only, no workspace).

Toolbox model: Craftsman CMST-98268-BK (consistent form factor since 2010, compatible with Kobalt, Husky, US General).

### Box 1 — Cutting
Cutting tools, oscillating tool, drilling. Featured in hole-drilling and oscillating tool videos.

### Box 2 — Clamping
Course fasteners, clamps, pneumatic tools, circular saw. 5 drawers.

### Box 3 — Instruments
USB cables, adapters, battery-powered instruments. **Requires climate control** — high priority for moisture management with desiccant in multiple drawers. If the lab catches fire, roll this box out first.

### Box 4 — Hammer/Forming
Forming, sanding, precision cutting, dusty tasks. Keep top surface clear for clamping work in adjustable bench clamps.

### Box 5 — Soldering
Wiring connections, crimping, soldering, fine work, heat tools. Built-in fume extractor, racks for common screwdrivers, adjustable mounts for lighting and hot air.

### Box 6 — Mechanics
Cutting tools, pliers, sockets, metal files. Many tools date back 15+ years. Drawers numbered 6.0-6.6 for potential tool database.

### Toolbox Modifications
- **Wood tops:** Pine 2x4s bonded with wood glue, optionally sealed with 2-part epoxy
- **Swinging frames:** Add tool hanging space on sides without protruding
- **Upper frames:** Create workspace for DIY stations (soldering, electrical testing)
- **Key caps:** 3D-printed designs on grabCAD — prevents snags and bent keys
- [Toolbox CAD model](https://grabcad.com/library/toolchest-1), [PDF manual](https://github.com/davidmalawey/openLab/blob/d9d88a53bd458391b65c19579c2a9006a9337a72/docs/2025_manual_RollingToolChest.pdf)

---

## 5. Stations

A station is formed by asking: **"What is the gap between the tool and useful work?"** Break that question into pieces, then arrange all pieces into one space.

> *Example:* A grommet press tool requires not just the tool but grommets, material to be grommeted, a surface to press against, lighting, and a staging area for finished parts. Arranging all of those creates the station.

### Soldering Station
- Structure: 30mm extrusion rack with 35mm DIN rail and printed tool holders
- **DIN-mounted power meter** monitors station-wide consumption — verify iron is sleeping, check device current draw
- Iron rests in insulated tube at back (stays hot, avoids burns, saves power)
- 120VAC outlet at station distributes power to heat gun, etc.
- **Iron recommendation:** Pinecil ($40, first choice) or TS100. Seek 80+ watts for <30 second heatup. Pinecil powers from USB-C PD at 20V/80W. Replaceable tips with embedded heating element and thermocouple.
- **Scope decision:** Through-hole components only (≥1.25mm). No SMD — turnkey boards are cheaper and easier.
- Key supplies: FEITA tips ($36), butane torch ($22), fume extractor ($30), Kaisi mat ($9), 120W USB power ($19), 0.8mm solder ($10), flux pen ($8), IGAN 330 flush cutters ($8), brass mesh cleaner ($10)

### Charge Station
- Wall-mounted shelf for USB-powered handheld tools, phones, battery cells
- USB-C outlet (micmi, $18) delivering up to 45W DC power, installed 2024
- XTAR VC4 battery charger for capacity testing, discharge tests, cell health monitoring
- XTAR PB2S modular power bank for portable charging (displays current in/out)
- Echo Dot for notifications and hands-free audio

### Admin Station
- Centered on Epson scanner (DS-510 since 2016, nearest current match: [Epson ES-400](https://amzn.to/3Qj0EIl))
- Key principle: **seamlessness between the world of data and the material world**
- Dymo 550 labeler ($120) for 5S labeling — fast, reliable, globally available compatible spools
- Brother PTD220 handheld label printer ($45)
- 3M Scotch TL902 thermal laminator ($60)

---

## 6. Storage & Organization

### Supply Shelves
- Two large shelving units subdivided for fasteners and categorized parts
- **Goal: collect or return any part in 10 seconds**
- ~1,000 unique parts per shelving unit
- Contains supplies only, not tools

### Hardware Bins
- Metric components (green-marked section) are highest priority
- **M2.5 and M6 are the default choices** for small and large fasteners
- Eliminate less-common sizes, maintain ability to produce them (cut 40mm to 35mm when needed)

### Bin Rack
- Modular design: 3030 metric extrusions, aluminum corner brackets, 35mm steel DIN rail, M6x12mm screws, standard industrial HDPE parts bins
- 10+ years of decision-making embedded in the design
- Wheels: outdoor sports wheels with 3D-printed adapter brackets
- Bin tops: 1/4in expanded PVC, lightweight, easy to clean, protects from dust
- [DIN rail 10-pack](https://amzn.to/437Bm7Z), [DIN cutter](https://amzn.to/4k7jZtP)

### Bin Type Hierarchy

| Bin Type | Size | Use | Storage Position |
|----------|------|-----|------------------|
| Plano Prolatch 3700 | 9x14in | Full parts categories (~50 unique components) | Flat or upright |
| Plano Prolatch 3500 | 5x9in | Lighter collections (fuses, clips) | Hung vertically on pegboard |
| Divider Bins (Akro-Mils) | 15x9x6in | Critical inventory, industrial grade ($15 each, last forever) | Shelves |
| Sterilite Clearview 6qt/15qt | Various | See-through grouped storage | Shelves |
| Zipper Pouches | Pencil bag size | Small grouped supplies | Hanging with hooks |

### Color Code System
Tools marked by last digit of size:

| Digit | Color | Mnemonic |
|-------|-------|----------|
| 0 | Black | — |
| 1 | White | — |
| 2 | Blue | "Two is blue" |
| 3 | Green | "Three is green" |
| 4 | Orange | — |
| 5 | Red | — |
| 6 | Silver | — |
| 7 | Yellow | — |
| 8 | Purple | — |
| 9 | Gold | — |

> *Example:* 13mm socket = green (3). 23mm socket also = green. 17mm wrench = yellow (7). Quick blot of yellow on a bolt during engine disassembly says "use 17mm wrench."

Tested and refined for 8+ years. Apply with enamel paint (Testors kit, $23) or nail polish. No sequences or bands — a quick blot anywhere works.

### Door Storage
- Tall items that don't fit in toolboxes
- All items must be fixed in all axes (forward, up, sideways) to prevent falling when door swings
- Limit items to avoid overloading hinges

### Hanger System
- TiltMount: 3D-printed bracket mounts 20mm beam on wall with gentle upward slope so straight hooks hold materials without slipping
- Compatible with Triton hook multipacks ($28) using M5x10mm fasteners
- [TiltMount CAD model](https://grabcad.com/library/tiltmount-1)

---

## 7. Key Tools

### 3D Printing
- **Focus on reliability over versatility**
- Three identical Flashforge Creator Pro printers (ABS, stacked vertically)
- 2026 addition: Flashforge AD5M Pro (~$550)
- **Recommended:** [Flashforge Adventurer 5M Pro](https://amzn.to/3J1W3KO) — metal frame, enclosure, balanced performance
- **Material:** ABS preferred for UV/sun tolerance, CA glue bonding, PVC compatibility, and toughness over PLA/PETG
- Slicer: Orca-Flashforge (open source with Flashforge settings)

### Cordless Power Tools
- **Ridgid brand** chosen for lifetime warranty and free replacement — competitive performance with DeWalt, Bosch, Milwaukee
- Four 3D-printed adapters for 18V DC: battery terminal, battery dummy, battery rack, battery jig (all on grabCAD)
- Full tool list: drill, driver, hammer drill, circular saw, jigsaw, reciprocating saw, router, cutout tool, heat gun, impact gun, blower, brad nailer, stapler, Dremel

### Hand Tools
- **Flush cutters:** IGAN 330 model only. Hardware store cutters are too bulky; stamped steel cutters bend with one forceful cut. [2-pack $14](https://amzn.to/42yBiwx)
- **Screwdrivers:** Westward precision drivers — PH0, PH1, 2.5mm slotted. [Printable holder on grabCAD](https://grabcad.com/library/mount_dr-1)
- **Calipers:** iGaging brand, [6-inch $47](https://amzn.to/4b0k6E1), [4-inch $35](https://amzn.to/4rRfsz2)
- **Drill guide:** [Kreg Brand $8](https://amzn.to/4kX5GsR)

### Safety & PPE
- **Safety glasses:** Color-coded, assigned to specific stations. Slot at each workstation marked with same color. [Pack of 12 in 6 colors $14](https://amzn.to/42pCrWB)
- **ANC headphones:** [Runolim $20](https://amzn.to/3RFOOJ2) — chosen for comfort over safety rating. Cancels steady noise from jigsaw/vacuum. Enhances focus and precision.
- **Gloves (3 types):**
  1. Cut resistant: Hyflex 11-561 [$13](https://amzn.to/4tYoaMR)
  2. Mechanics: MCR Safety 919 [$25](https://amzn.to/48BSqom)
  3. Chemical: Showa 719B or Honeywell 101V [$25/12-pair](https://amzn.to/4chr7Cc)
- All from reputable manufacturers with documented part numbers and datasheets

### Software Stack

| Purpose | Application | Notes |
|---------|-------------|-------|
| Scanning | NAPS2 | Free, open source, lightweight |
| PDF editing | PDF Xchange Editor | Paid, most full-featured |
| Images/Screenshots | ShareX | Open source, tons of tools |
| Diagrams | Draw.io | Open source, SVG capable |
| 3D Slicing | Orca-Flashforge | Open source, Flashforge built-in |

### PC Workstation
- AMD Ryzen 7 3700x CPU
- AMD Radeon Pro WX4100 GPU (chosen over RTX2060 — lower cost, lower power, better CAD performance)
- Samsung 980 Pro M.2 SSD
- 32GB Corsair Vengeance RGB Pro 3200 RAM
- Corsair RM750x PSU
- Dual HP 27h monitors

---

## 8. Electronics Setup

### Key Devices
Microcontrollers: ESP8266, ESP32, ESPWROOM (all with wiring diagrams)
Sensors: soil moisture (LM393), IR motion (AM312), temp-humidity (SHT31), ambient light (TLS2591), thermistor (DS18B20), flow sensor (FL-608)
Actuator drivers: DRV8825 stepper, A4988, WS2811 addressable LED

### Bin Organization
Organize in **action-based bins** (survived 3-8 years without label changes):
- **MCU** — microcontroller boards
- **Sensors 1** — popular, well-documented, single-semester friendly (SHT31, soil moisture, IR motion)
- **Sensors 2** — higher-effort items requiring more integration (GPS, SD card, strain gauge). Advise students to avoid for single-semester projects.
- **Actuators** — relays, motor drivers, MOSFETs, PWM generators, audio amplifiers
- **Dupont** — standard removable cable ends for all DIY projects (use other connector types only for water resistance, shock, heat)
- **Battery** — 18650 cells, contacts, trays, BMS boards
- **Servos** — RC-style servo motors (under $10 each, include metal geartrain, analog feedback, servo horns)
- **Solder** — through-hole supplies only
- **Switches** — power switches from micro limit to large enclosed roller-lever
- **Terminals** — 10A+ rated connectors (Anderson, spade terminals)
- **DIN Rail** — best method for terminating/routing power cables (vs signals)
- **LED Lights** — small to full spools
- **Connectors** — major power input sockets (Schurter brand)
- **Pigtail** — pre-made connector+cable assemblies and recovered cables

### Design Standards
- **18 gauge** standard wire for power, 16 gauge for 18V battery projects
- Keep current **below 10A** for easy terminal selection
- **DIN rail** for any project above 50 watts of power
- **Dupont connectors** as default for signal wiring
- MCU costs are now so low that device + cables + sensors + 3D printed enclosure costs less than engineering time to write the software

### Servo Motors
The most sophisticated complete control system with mechanical actuator under $20. Standard 50Hz/20ms pulse at 5V, compatible with all popular MCUs. Failure mode engineered: horn teeth are weaker than output gear, so the expendable part breaks in a crash. [HowToMechatronics tutorial](https://howtomechatronics.com/how-it-works/how-servo-motors-work-how-to-control-servos-using-arduino/)

---

## 9. Materials & Methods

### Bonding
With bonds that exceed material strength, two parts can become one part after manufacturing. Over 10 years of adhesives research. Test with standardized "testbar" geometry for shear loads — if you can crack parts free with arm strength, it's likely below 40 lbs on the pull test. [Bonding Guide PDF](https://github.com/davidmalawey/openLab/blob/d06d0a1b5ddcd02dc7e80e1ec11b800954070d18/docs/2025_bondingGuide.pdf)

### OTP Parts (Off-The-Print)
Parametric 3D printed designs with recurring instances. Each instance is unique but driven by refined parametric models. Similar to OTS (off-the-shelf): easy to grab-and-go, low cost, wide application, globally available via grabCAD.

> *Example:* Hinge_V2 used first on toolboxes for nested racks, then reused with adjusted geometry to hold datasheets for video capture. Each reuse gains a solution unavailable from off-the-shelf parts.

### Printegration
Designing parts using 3D printing plus all commercial off-the-shelf components. Doubles value over plain parametric parts by including parameters derived from the mating part. Key designs: sleeves (tested to 600 lbs with superglue on fiberglass rebar), hinges (±90°, multiple beam types), bearings (print-in-place, parametric), mandrels (150+ lbs shear on EMT conduit).

### Tubing
Polyethylene tubing (3/8 x 1/4 inch OD/ID) — used hundreds of ways:
1. Hinge pins for printed parts
2. Washers for M5-M8 assemblies
3. Springs (cut short lengths)
4. Gap fillers in assemblies
5. Pneumatic air lines
6. Drinking water lines (safe)
- [3/8in $11/25ft](https://amzn.to/3YCALYw), [1/4in $14/40ft](https://amzn.to/49BKKSG)

### Push-Fit Connectors
Tool-free assembly, 200 PSI tolerance, reusable without damage, tubes rotate without breaking seal. Tested 7+ years with zero leaks. Replace NPT fittings, tapping, and thread-sealing tape for small-volume fluid and air routing.

---

## 10. Documentation & Meta

### Image Standards
- Format: .jpg (better compression, supports tags)
- Aspect ratio: square (most versatile for online posting, survives cropping)
- Resolution: 2048x2048
- Target: ≤350KB
- Include tags in the image for traceability
- File naming: `img_descriptor1.jpg` (prefix + numbered suffix)

### CAD Documentation
- All models tagged with keyword "openlab" on GrabCAD
- STEP-AP14 format priority (color rendering on web viewers)
- STL files: one per printable part, Z-axis up indicating print direction, 1-digit revision number in filename
- No hidden postprocessing steps
- Include crucial mating components as simplified geometry
- GrabCAD chosen for: engineering focus, collaboration tools, version control, wide file type support

### File Management
- All files below 25MB (GitHub max)
- Videos on YouTube (select "unlisted" for non-public), no file size limit
- Every file in the repo serves a purpose — delete duplicates and undescribed files

### When a Part Becomes a Project
A design becomes a project when: A) documentation doesn't fit within one CAD post, or B) intended value is outside the part's performance. Projects need use cases, key suppliers, benchmarked OTS variants, application videos, and naming conventions.

### Manuals
Tool manuals stored as PDFs: simplified (non-English removed), tagged for search, compressed, OCR-enhanced for text search, bookmarked at key sections. Notes from lab use added as additional pages with author initials and dates.

---

## 11. Community & Resources

### Related Projects

| Project | Link | Domain |
|---------|------|--------|
| OpenAir | [qr.net/openairproject](https://qr.net/openairproject) | Air, pressure, flow |
| OpenArm | [qr.net/openarmproject](https://qr.net/openarmproject) | Robotic arms (10-year goal) |
| OpenBox | [qr.net/openboxproject](https://qr.net/openboxproject) | Steel box designs |
| OpenGrow | [qr.net/opengrowproject](https://qr.net/opengrowproject) | Hydroponics, aquaponics |
| OpenJar | [qr.net/openjarproject](https://qr.net/openjarproject) | Jars, threads, seals |
| openME | [qr.net/openmeproject](https://qr.net/openmeproject) | Free ME degree (in-progress) |
| OpenSpin | [qr.net/openspinproject](https://qr.net/openspinproject) | Parametric bearings |
| SCUTTLE Tech | [qr.net/scuttleproject](https://qr.net/scuttleproject) | SCUTTLE robot designs |
| SCUTTLE Mini | [qr.net/scuttlemini](https://qr.net/scuttlemini) | Miniature mobile robot |
| SCUTTLE Nigeria | [qr.net/scuttleafrica](https://qr.net/scuttleafrica) | University robotics lab, Lagos |

### Community
- [Discord](https://discord.gg/Napn9mhd43)
- [YouTube](https://www.youtube.com/@davidmalawey) — 400+ engineering videos
- [Amazon supply lists](https://www.amazon.com/shop/davidmalawey)
- [SCUTTLE Robotics Resources](https://www.scuttlerobot.org/resources/)
- [David Malawey's homepage](https://davidmalawey.com)

### Reference Materials
Engineering references kept in the repo:
- NFPA70 Electrical Standards
- Gates Belt Design Guide
- Koyo Bearing Guide
- US Marines MOLLE Equipment Guide
- Forest Products Lab Wood Handbook
- [Toyota Production System Handbook PDF](https://github.com/davidmalawey/openLab/blob/a250af57f0167144ccfb82e9223d3464c2ee7e07/docs/2026_ToyotaHandbook.pdf)

### Research Approach
Use distributors (McMaster, AutomationDirect) as research partners, not just stores. They hire engineering teams to understand applications — their expertise is often deeper than the customer's. Find catalogs from the longest-standing manufacturers to understand the full span of technical variations.

---

## Caveats

The following aspects of OpenLab have **not yet been independently validated** (tracked as OUT beliefs in the EEM):
- No external lab has successfully replicated the full OpenLab setup
- Community transferability of the methodology is unproven
- The lab still depends significantly on David Malawey as primary knowledge holder
- Printegration methodology is not yet mature enough for independent adoption
- Electronics designs have not been validated for production-ready replication

This guide is a reference, not a proven replication manual. Use it as a foundation and expect to adapt.
