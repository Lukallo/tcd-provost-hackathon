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
