# Venture ideas: big ideas with a business model

Each idea has a **thesis** (the insight), **the business**, **who pays**, **why now**, and **who's nearby** (competitors and precedents).
Rule of thumb: the strongest environmental businesses are ones where a **regulation or cost forces someone to pay**.
Goodwill alone doesn't pay the bills.

> Regulation dates are from memory. EU timelines have been moving (several were delayed in 2025), so check each one
> before it goes in a pitch.

## Tier 1: someone is already forced to pay

### 1. Trust layer for nature credits
- **Thesis:** Carbon and biodiversity credits are only worth what their proof is worth. Verification (MRV: measurement, reporting
  and verification) is the bottleneck, and it's priced for big projects.
- **Business:** Cheap ground sensors + satellite + AI give *continuous* proof that a bog is wet, a hedge is alive or a forest is
  standing. Sold per hectare per year.
- **Who pays:** credit developers, registries, buyers who need to prove their credits are real.
- **Why now:** the EU Carbon Removal Certification Framework (CRCF, adopted 2024) is creating certified EU removals. Credit
  buyers are under fire over credits that turned out not to be real.
- **Nearby:** Pachama, Sylvera (satellite ratings) → **ground truth for small, wet, non-forest land.** Smoulder hardware fits here.

### 2. Peatland rewetting developer
- **Thesis:** Ireland has a lot of drained peat that emits carbon. Each landowner is too small to sell credits on their own.
- **Business:** Sign up many small landowners, run the rewetting, sell the credits, and share revenue with the landowners.
  Monitoring comes from #1.
- **Who pays:** corporate buyers of carbon removals/avoidance; landowners get recurring income.
- **Why now:** CRCF, national peatland targets. The UK's Peatland Code shows the model works.
- **Nearby:** Bord na Móna (its own land), UK Peatland Code projects → **aggregating private small holdings.**

### 3. Digital Product Passport as a service
- **Thesis:** The EU will require products to carry a digital passport (materials, repairability, origin). SMEs have no
  idea how to do it.
- **Business:** Upload your bill of materials + supplier documents → get a compliant passport + QR code. SaaS per product.
- **Who pays:** manufacturers and brands selling into the EU.
- **Why now:** the Ecodesign Regulation (ESPR, 2024) and the Battery Regulation's battery passport (from Feb 2027 for
  EV/industrial batteries; verify).
- **Nearby:** Circularise, Arianee, others → **SME-first, Irish manufacturing and medtech niche.**

### 4. Deforestation-free proof for smallholders
- **Thesis:** EU importers of coffee, cocoa, cattle, soy, palm, rubber and wood must prove their goods aren't linked to
  deforestation, down to the plot. Smallholders risk being dropped because they can't prove it.
- **Business:** A phone app maps the plot's boundary, and satellite checks give a compliance certificate. Importers pay; farmers get
  it free and keep market access.
- **Why now:** EUDR (application was delayed; check the current date).
- **Nearby:** Satelligence, Meridia → **built for farmer cooperatives, priced for importers.**

### 5. Textile feedstock sorter
- **Thesis:** EU countries must collect textiles separately (since 2025), and producer responsibility for textiles is
  coming. Sorting mixed clothing into recyclable fibre is the bottleneck.
- **Business:** An automated near-infrared sorting line; sell sorted fibre to recyclers and charge producers' compliance schemes
  per tonne.
- **Nearby:** Fibersort, Sysav → **an Irish/UK regional hub; Ireland currently exports most of its used textiles.**

### 6. Reuse infrastructure (washing hub as a service)
- **Thesis:** The EU Packaging Regulation (PPWR) brings reuse targets for 2030. Brands want reusable packaging, but nobody
  wants to run the dirty middle: collection, washing, return.
- **Business:** A shared washing hub and reverse logistics for cafés, caterers and events, charged per cycle.
- **Nearby:** Loop (consumer brand), Recup (Germany) → **back-end infrastructure, not a consumer brand.**

## Tier 2: saves money, which is easier to sell than goodwill

### 7. Soaking up wasted wind
- **Thesis:** Ireland has to turn off wind turbines on windy nights because the grid can't absorb the power (curtailment). That power is wasted.
- **Business:** A smart controller that heats hot-water tanks and storage heaters when wind is being curtailed. Revenue share
  with energy suppliers and grid flexibility payments.
- **Nearby:** Octopus-style smart tariffs, Mixergy → **targeted at the Irish curtailment problem, and works with existing immersion heaters.**

### 8. Compute that heats homes
- **Thesis:** Data centres throw heat away; homes pay to make it.
- **Business:** Servers inside home hot-water tanks; sell compute to businesses; the household gets free hot water.
- **Nearby:** Heata (UK) does exactly this → **Ireland is a natural market: lots of data-centre demand and pressure on grid capacity.**

### 9. Washing machines as a service
- **Thesis:** Pay per wash, so the manufacturer profits from machines that last and get repaired.
- **Business:** Durable machines on a monthly subscription for rentals, student housing and landlords; refurbish
  them between tenants.
- **Nearby:** Bundles (Netherlands) → **landlords as the channel: Irish rentals are often furnished, so landlords buy appliances in bulk.**

### 10. Refurbished business laptops
- **Thesis:** Companies replace laptops every 3–4 years, and most of the emissions are from making them. The EU Right to Repair directive
  (2024) helps repair.
- **Business:** Lease refurbished laptop fleets with a warranty and an emissions-saving report for ESG disclosures.
- **Nearby:** Back Market (consumer), Grover (rental) → **B2B fleets with ESG reporting included.**

## Tier 3: a waste turned into two revenue streams

### 11. Invasive species → biochar → credits
- **Thesis:** Clearing rhododendron in places like Killarney is an expensive cost. Turn the cleared plants into biochar.
- **Business:** Paid to clear (fee) + sell biochar to farmers (product) + sell carbon removal credits (CRCF). **Three revenue
  streams from one waste.**
- **Nearby:** biochar startups generally → **feedstock that's free, and you're paid to take it away.**

### 12. Wildfire liability protection for utilities and railways
- **Thesis:** Power lines and railways spark fires and carry huge liability. Detection is cheap compared with lawsuits.
- **Business:** A sensor network + risk score along the line, sold to utilities, rail operators and their insurers;
  pairs with parametric insurance (pays out automatically when sensors confirm a fire).
- **Nearby:** Dryad already targets this → **pick the European railway niche + bundle insurance.**

### 13. Insurance that pays when the data says so
- **Thesis:** Farmers and small businesses can't get affordable flood, drought or fire cover; claims assessment is the
  costly part.
- **Business:** Parametric policies that pay automatically when a sensor or satellite threshold is hit. Earn as a managing general
  agent (MGA) or data provider to insurers.
- **Nearby:** Descartes Underwriting, FloodFlash (UK) → **Irish agriculture + upland fire.**

---

## Best fit for the hackathon

| Idea | Profit case | Can we prototype in a day? | Judge appeal |
|---|---|---|---|
| **1 + 2 together** (rewetting developer with its own monitoring) | High: credits + recurring data revenue | Yes: sensor + dashboard + revenue model | Strong; very Irish |
| **11** (rhododendron → biochar → credits) | High: three revenue streams | Yes: business model canvas + flow | Very memorable |
| **7** (curtailed wind → hot water) | Medium–High | Yes: ESP32 + relay + a wind-data feed | Clear and tangible |
| **3** (product passport SaaS) | High, but crowded | Yes: a mock-up | Less "human-centred" |

For the pitch: **who pays, why they must pay now, unit economics on one slide** (cost per hectare/device vs. revenue
per hectare/device), then the pilot.
