# Idea brainstorm

Ideas can be anything environmental. They don't have to be campus-based. Each idea lists **what already exists**,
because judges will ask, and the Innovation score depends on having a clear answer.

Scores are first-pass gut calls (1–5) weighted by the judging criteria. Redo them with the team.
Impact 25% · Alignment 20% · Innovation 20% · Feasibility 20% · Human-centred 15%.
Numbers marked *(verify)* came from memory, not a source; check them before they go in a pitch.

## Shortlist

| # | Idea | Area | Imp | Align | Innov | Feas | HCD | **Weighted** |
|---|---|---|---|---|---|---|---|---|
| 1 | **Smoulder** — peat & upland fire watch ([deep dive](WILDFIRE.md)) | Climate & Nature | 4 | 5 | 4 | 3 | 3 | **3.85** |
| 2 | Bog water-table sensors → rewetting payments | Climate & Nature | 4 | 5 | 4 | 3 | 3 | **3.85** |
| 3 | Farm-gate nitrate alert | Climate & Nature | 4 | 5 | 3 | 3 | 4 | **3.80** |
| 4 | Ghost-gear tag & bounty | Climate & Nature | 4 | 5 | 3 | 3 | 3 | **3.65** |
| 5 | Small-source waste-heat matchmaker | Sustainable Communities | 4 | 4 | 3 | 3 | 3 | **3.45** |
| 6 | Vape battery take-back | Responsible Consumption | 3 | 4 | 3 | 4 | 3 | **3.40** |

---

## 1. Smoulder — wildfire detection for peat and uplands
Silvanet is built for forests: gas sensors mounted on trees, about 1 per hectare. Ireland's fires are on open heath, gorse and
bog, many are deliberate, and drained peat can burn *underground* for weeks. The idea is ground stakes with a soil
temperature probe and a CO sensor, a wind-aware sparse network, and a register for legal controlled burns so they don't trigger false alarms.
**Full write-up: [`WILDFIRE.md`](WILDFIRE.md).**

## 2. Bog water-table sensors → rewetting payments
- **Problem:** Rewetting drained peatland is one of Ireland's biggest climate levers, but proving that a bog is actually wet
  (and so storing carbon) needs monitoring that small landowners can't afford.
- **Idea:** A cheap water-table logger plus a farmer dashboard that turns readings into evidence for agri-environment or
  carbon payments.
- **Exists:** research-grade dataloggers; national peatland programmes. **Angle:** priced for a single farmer, and the result
  is a payment, not just a dataset.
- **Prototype:** a pipe in a bucket of wet compost with an ultrasonic or pressure sensor, and a dashboard mock-up showing "€/yr earned".
- *Pairs naturally with #1.* The same stake does both jobs, which makes this a strong combined pitch.

## 3. Farm-gate nitrate alert
- **Problem:** Agricultural nitrogen is the main pressure on Irish rivers. EPA reports put roughly half of rivers below
  good ecological status *(verify)*.
- **Idea:** A low-cost nitrate test strip + phone camera reader for farm drains, linked to rainfall forecasts. It tells the
  farmer "don't spread slurry this week, here's why" in plain language.
- **Exists:** EPA monitoring stations (sparse), lab tests, the ASSAP advisory programme. **Angle:** farm-level, same-day, and
  framed around timing decisions the farmer already makes.
- **Prototype:** a phone flow + a printed strip colour chart.

## 4. Ghost-gear tag & bounty
- **Problem:** Lost and abandoned fishing gear keeps catching marine life for years. A widely cited figure is about 640,000 t
  a year globally *(verify)*.
- **Idea:** Cheap ID tags on nets + a deposit scheme. Fishers pay a small deposit per tagged net and get it back when the net is returned. Anyone who
  recovers a lost tagged net gets a bounty.
- **Exists:** smart-buoy trackers (e.g. Blue Ocean Gear), Fishing for Litter programmes. **Angle:** the deposit/bounty
  economics, not the hardware.
- **Prototype:** a service blueprint + a tag mock-up + the deposit maths for one Irish harbour.

## 5. Small-source waste-heat matchmaker
- **Problem:** Data centres use around a fifth of Ireland's electricity *(verify: CSO)* and give off heat. Tallaght's district heating
  already uses heat from a data centre, but smaller sources (supermarket fridges, server rooms, breweries) are ignored.
- **Idea:** A map + calculator that matches small heat sources with nearby heat users (pools, apartment blocks,
  greenhouses) and estimates the payback.
- **Exists:** large district-heating projects and national heat studies. **Angle:** small, local matches that don't need a city scheme.
- **Prototype:** a map of one Dublin neighbourhood with 3 real matches worked out.

## 6. Vape battery take-back
- **Problem:** Disposable vapes contain lithium batteries that end up in bins, where they can start fires in waste trucks and
  recycling plants.
- **Idea:** Shop-counter collection + deposit, plus a supply chain that harvests the cells for reuse.
- **Exists:** WEEE take-back obligations; check current Irish/EU rules on disposable vapes before pitching.
  **Angle:** making return easy at the point of sale, and the value of the recovered cells.
- **Prototype:** counter-bin mock-up + flow from return to reuse.

---

## Picking one
Before choosing, ask these about each idea:
1. **Can we name the user and talk to them before 24 Oct?** If not, Human-centred design suffers.
2. **Can we show something in 20 seconds?** A working sensor or a sharp storyboard beats slides.
3. **Can we name the incumbent and say in one sentence why they don't solve it?**
4. **Is there a number for the impact?** (hectares, tonnes, €, people)

Smoulder (#1, ideally merged with #2) passes all four if someone on the team can do basic electronics and we get one ranger or
farmer conversation in before the day.

---

# 25 ideas

Format: **Idea**: what it is. *Exists:* what's out there → **our angle**. *Prototype:* what to show on the day.

## Climate & Nature (SDGs 6, 13, 14, 15)

1. **Smoulder**: ground stakes that catch peat and upland fires, including underground smoulder, plus a register for legal burns.
   *Exists:* Silvanet (tree-mounted, built for forests) → **open landscape, underground fires, and sorting legal from illegal burns.** *Prototype:* ESP32 + CO sensor + temperature probe in compost, with an incense-stick demo. See [`WILDFIRE.md`](WILDFIRE.md).
2. **Bog water-table → payments**: cheap logger that proves a rewetted bog is wet, so the landowner gets paid.
   *Exists:* research dataloggers → **priced for one farmer; the output is a payment claim.** *Prototype:* pipe in a bucket + dashboard showing €/yr.
3. **Farm-gate nitrate alert**: test strip + phone camera reading on farm drains, combined with the rain forecast → "don't spread slurry this week".
   *Exists:* sparse EPA stations, lab tests → **same-day, on the farm, tied to a decision the farmer already makes.** *Prototype:* phone flow + strip colour chart.
4. **Ghost-gear deposit**: tagged fishing nets, a deposit paid back when the net is returned, and a bounty for anyone who recovers a lost one.
   *Exists:* smart buoys, Fishing for Litter → **the economics, not the hardware.** *Prototype:* deposit maths for one Irish harbour.
5. **Hedgerow sound check**: cheap audio recorders + automatic bird and bat ID give farmers evidence for results-based biodiversity payments.
   *Exists:* AudioMoth, BirdNET (research tools) → **packaged as evidence for a farmer's payment.** *Prototype:* run BirdNET on a recording from a hedge on campus.
6. **Rain-garden street kits**: planters that soak up roof runoff, so less rain overloads sewers and causes overflows into rivers and Dublin Bay.
   *Exists:* council sustainable drainage schemes → **one street at a time, crowdfunded, with a counter showing litres kept out of the sewer.** *Prototype:* street storyboard + a downpipe-to-planter model.
7. **Invasives work-party app**: map rhododendron or knotweed patches and fill volunteer clearing days for them.
   *Exists:* iNaturalist and Biodiversity Ireland records (they map but don't organise the work) → **turning a map pin into a filled work party.** *Prototype:* app mock-up for Killarney.
8. **Seagrass seed-bag kits**: volunteers sew and plant seed bags to restore seagrass meadows that store carbon.
   *Exists:* Project Seagrass (UK) → **an Irish coastal version run through clubs and schools.** *Prototype:* kit + volunteer journey.

## Responsible Consumption (SDGs 2, 12)

9. **Vape battery take-back**: deposit + return bin at the shop counter; cells are harvested for reuse.
   *Exists:* WEEE take-back rules → **return at the point of sale, and value from the recovered cells.** *Prototype:* bin mock-up + flow from return to reuse.
10. **Canteen bin camera**: cheap camera over the waste bin in school or hospital canteens measures what gets thrown away, so kitchens can adjust portions.
    *Exists:* Winnow (commercial kitchens, priced for them) → **a version cheap enough for public canteens.** *Prototype:* photos of a tray → a "waste by dish" chart.
11. **One-cup Dublin**: a single deposit cup accepted at any café, instead of each chain running its own scheme.
    *Exists:* separate schemes for each brand → **one cup that works across the city.** *Prototype:* cup + return-point map + café cost maths.
12. **Salvage marketplace**: materials taken from demolitions and renovations (doors, radiators, timber), listed for builders and DIYers.
    *Exists:* Rotor DC (Belgium) → **an Irish version during the housing build-out.** *Prototype:* listing flow + one real demolition priced.
13. **Baby gear library**: rent prams, slings and cots through maternity hospitals; they're used for months and then discarded.
    *Exists:* general libraries of things → **reaching parents through the hospital, when they need the gear.** *Prototype:* service blueprint + pricing.
14. **Repair or replace?**: photograph a broken appliance → estimated repair cost, CO₂ saved, nearest repair café.
    *Exists:* repair cafés, iFixit → **the decision at the moment it's made.** *Prototype:* phone flow for 3 appliances.
15. **Debs & wedding wardrobe**: rent or swap outfits worn once, run with schools and alterations shops.
    *Exists:* some rental shops → **a school-based exchange with tailoring included.** *Prototype:* storyboard + one school's numbers.

## Sustainable Communities (SDG 11)

16. **Waste-heat matchmaker**: match small heat sources (supermarket fridges, server rooms, breweries) with nearby heat users.
    *Exists:* large district heating (e.g. Tallaght) → **small local matches.** *Prototype:* map of one neighbourhood with 3 matches.
17. **Street heat-pump group buy**: neighbours on one street retrofit together to cut survey, install and grant-paperwork costs.
    *Exists:* SEAI one-stop shops (one house at a time) → **one street at a time.** *Prototype:* street sign-up flow + cost-per-house curve.
18. **Derelict → meanwhile use**: map of vacant and derelict buildings matched to community groups for temporary use.
    *Exists:* derelict sites registers, vacancy taxes → **matching buildings to users, not just listing them.** *Prototype:* map + one building's "meanwhile" plan.
19. **Rural ride-share for older people**: volunteer drivers for trips Local Link buses don't cover.
    *Exists:* Local Link, informal lifts → **booking by phone call, not an app.** *Prototype:* phone script + matching flow.
20. **Shared cargo bikes for small shops**: a pool of e-cargo bikes shared by high-street shops for local deliveries.
    *Exists:* courier companies → **shared ownership between shops.** *Prototype:* shop journey + cost vs. van.
21. **School-roof solar for the street**: solar on a school roof, with neighbours buying the surplus power and the school earning from it.
    *Exists:* micro-generation export payments → **neighbours sharing in it.** *Prototype:* one real school roof modelled.

## People & Wellbeing (SDGs 3, 4, 5, 10)

22. **Weather-triggered check-ins**: heatwaves or cold snaps automatically start calls to isolated older people and alert a neighbour.
    *Exists:* ALONE and befriending services → **triggered by the weather, so contact happens when risk is highest.** *Prototype:* call script + alert flow.
23. **Classroom CO₂ traffic light**: a cheap CO₂ sensor with a red/amber/green light tells the class when to open a window.
    *Exists:* CO₂ monitors given to schools → **designed for children to act on, not just a number on a display.** *Prototype:* working sensor + light.
24. **Climate anxiety → local action**: tell it your skills and free hours, get matched to a nearby climate project.
    *Exists:* volunteering sites → **built for young people who feel anxious about climate, with results shown back to them.** *Prototype:* matching flow mock-up.
25. **Step-free nature**: trails mapped and rated for wheelchairs, buggies and limited mobility.
    *Exists:* general trail apps → **access details collected by people who use them.** *Prototype:* 3 Dublin trails mapped.
