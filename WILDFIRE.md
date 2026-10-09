# Wildfire detection: can we beat Silvanet?

## What Silvanet already does
Dryad Networks (Berlin) makes the Silvanet system:
- Solar-powered sensors mounted on trees. A metal-oxide gas sensor picks up hydrogen, CO and VOCs, and a small ML model
  runs on the device, so it "smells" a fire while it is still smouldering, before there are flames or a visible plume.
- Sensors pass data along a LoRa mesh to border gateways and then to the cloud. The Gen 4 Pro (May 2026) can send
  straight to a satellite, so it needs no gateway.
- Dryad says it has over 50 customers and more than 30,000 sensors made and deployed. In the XPRIZE Wildfire finals, its sensors
  triggered the Silvaguard drone to find and attack a small fire on its own (company claim).
- **Known limits:** for fast detection the CEO quotes about 1 sensor per hectare (1 per 5 ha overall). Sensors are only on trees,
  and solar power is weak under the canopy. Almost all performance data comes from Dryad itself. Other players: N5 Sensors (US,
  needs LTE coverage, 1–2 mile range claimed), OroraTech (satellites), Pano AI (cameras). Voltree tried
  tree-powered sensor nodes in 2008–09 with the US Forest Service.

**Honest take:** a team can't out-engineer a well-funded company with 30k units deployed in one day, and judges will know
Dryad. "Silvanet but better" loses on Feasibility and Innovation. **"The case Silvanet wasn't built for"** wins.

## The gap: Ireland's fires aren't forest fires
- In 2025, Ireland burned **4,355 ha** (EFFIS, 31 fires) or **5,013 ha** (EU JRC, 99 fires). That's the highest since 2017,
  up from about 200 ha in 2024. Most of it was on **open upland heath, gorse and bog**, not forest.
- About **a third of the burned area was on Natura 2000 protected sites** (about 54% over 2015–2025 in one cross-border analysis).
- Fires cluster in **March–May**. Many are **deliberate**: 283 farmers were fined for illegal burning in 2025, and NPWS said
  the Dublin/Wicklow Mountains fire was "lit intentionally".
- **Drained peat can smoulder underground for days or weeks**, releasing carbon that took thousands of years to store.

There are no trees to mount on, little canopy, the fire can be *underground*, and the main cause is human. A
tree-mounted, forest-tuned gas network doesn't fit this well.

## Concept: "Smoulder" — ground-level fire watch for peatlands and uplands

**Problem statement (draft):** NPWS rangers and local fire services in Ireland's uplands learn about fires late, after
they have spread across protected heath and bog. Drained peat can keep burning underground for weeks after the surface
fire is out, releasing stored carbon, and nobody is watching it.

**Three layers:**
1. **Ground stakes, not tree tags.** A low-cost stake driven into peat. It has a soil temperature probe at 10–30 cm (to catch
   underground smoulder) and a CO/VOC sensor at the surface. It is solar-powered (no canopy to block the sun on open moorland) and
   connects over LoRaWAN or satellite. The same stake logs **water-table depth**, which shows how dry the bog is and so the fire
   risk *before* ignition. That data is also what peatland rewetting projects need to prove carbon savings, which gives a
   second revenue stream.
2. **Sparse, wind-aware placement.** Use fewer nodes than one per hectare. When several stakes register a rise, combine it with
   wind direction to work back to the likely source (simple plume triangulation). Put stakes densely along tracks, car parks and
   the edges of farm land, where ignitions start, and sparsely elsewhere.
3. **Burn register, so legal burns don't cause false alarms.** Farmers log a planned controlled burn (location and date) in a
   simple form or by SMS. An alert inside a registered burn zone during its window is tagged "expected". Anything else goes
   straight to the ranger. This also gives NPWS and Gardaí data on burns that weren't registered.

**Why it's different from Silvanet:** it targets open landscape instead of forest and catches underground smoulder as
well as surface fires. It measures fire risk (bog dryness), not just ignition. It sorts legal from illegal burns. And
it pays for itself twice, through fire detection and peatland carbon monitoring.

## Scoring (first pass)
| Impact 25% | Alignment 20% | Innovation 20% | Feasibility 20% | Human-centred 15% | Weighted |
|---|---|---|---|---|---|
| 4 | 5 (SDG 13, 15) | 4 | 3 | 3 → raise with interviews | **3.85** |

The weakest score is human-centred design. Fix it before the day by talking to the actual users (list below).

## Prototype on the day (pick one or both)
- **Working stake (hardware person on the team):** ESP32 + CO sensor (e.g. MQ-7 or an electrochemical cell) + DS18B20 waterproof
  temperature probe in a jar of compost. Light an incense stick next to it and show the alert on a phone. That's a 20-second demo
  that judges remember.
- **Service storyboard:** ranger's phone gets an alert → map shows the likely source cone from wind → checks the burn register →
  "unregistered" → dispatch. Add a second panel showing a farmer registering a burn by SMS.
- **Map mock-up:** stake placement on a real site (e.g. Wicklow Mountains National Park or Mount Leinster), with tracks and car
  parks highlighted.

## Key assumptions to test
| Assumption | How to test | Risk |
|---|---|---|
| Soil temperature probes catch underground peat smoulder early enough to matter | Look up peat-fire science (temperature profiles, depth) | High |
| A sparse network plus wind data locates fires well enough | Simple simulation, or the literature on plume source localisation | High |
| Metal-oxide CO sensors can run on solar power; their heaters draw a lot of current | Check the datasheets, look at low-power electrochemical options | Medium |
| Rangers would act on an alert (not just more noise) | Interview NPWS / county fire service | High |
| Farmers would register burns if it's SMS-easy | Interview 3–5 upland farmers or an IFA hill farming contact | Medium |
| Peatland rewetting projects would pay for water-table data | Ask Bord na Móna / rewetting project or NPWS peatland team | Medium |
| Cost per stake is low enough to deploy at scale | Price the parts (BOM), compare with Silvanet's reported ~$50 per sensor (2023) | Medium |

## People to contact before 24 Oct
- NPWS rangers (Wicklow Mountains National Park)
- Wicklow Uplands Council / local fire brigade
- Peatland researchers at Trinity (Botany / Geography) and anyone on the Bord na Móna rewetting programmes
- One or two upland farmers (Teagasc or IFA contacts)

Ask them: *"Tell me about the last fire you dealt with. How did you find out, and how long had it been burning?"*

## Sources
- Dryad FAQ — https://www.dryad.net/faq
- Gigaom interview with Dryad CEO (sensor density) — https://s.gigaom.com/?p=1037636
- Dryad Gen 4 Pro launch (May 2026) — https://www.businesswire.com/news/home/20260510819235/en/
- Dryad XPRIZE finals (July 2026) — https://secure.businesswire.com/news/home/20260707802818/en/
- ABI Research on wildfire IoT (sensor price) — https://www.abiresearch.com/market-research/insight/7782559-the-smart-way-to-prevent-wildfires-an-iot-
- N5 Sensors in San Mateo County — https://www.ktvu.com/news/50-wildfire-sensors-installed-throughout-san-mateo-county
- Voltree tree-powered sensors — https://cleantechnica.com/2008/09/22/forest-fire-warning-system-derives-power-from-trees/
- Ireland 2025 burned area (JRC) — https://www.laois-nationalist.ie/over-5000-hectares-burnt-in-ireland-during-eus-worst-year-for-wildfires_arid-93549.html
- Natura 2000 share, peat smoulder — https://www.europeandatajournalism.eu/?p=261826 · https://www.irishexaminer.com/lifestyle/outdoors/arid-41877212.html
- Farmers fined for illegal burning — https://www.agriland.ie/farming-news/tag/gorse-fires
