# Wildlife Strike Analytics — Results Report


## 1) Key Findings
1. **Location & traffic density matter most.** High-incidence areas cluster around **large airports, coastal regions, and major migration routes**. Inland areas with lower bird populations and fewer operations show substantially fewer strikes.  
2. **Flight phase is the dominant operational driver.** **Approach and landing-roll** phases carry the highest risk and most severe damage, aligning with lower altitude and speed during terminal operations.  
3. **Seasonality and migration.** Year-over-year patterns exhibit **seasonal fluctuations** and **noteworthy peaks** in specific months/years, consistent with migration cycles near busy corridors.  
4. **Speed profile.** A sharp strike concentration appears around **140–160 knots**, typical of approach/landing; **events above 300 knots are rare**, indicating high-altitude encounters are uncommon.  
5. **Species & environment.** Commonly hit species and **airport-adjacent habitats** (wetlands, coasts, agricultural land) elevate risk; hotspots over open ocean are minimal, reinforcing the proximity effect.  
6. **Modeling takeaway.** A simple linear regression trained on historical counts gives reasonable **short-term trend** projections but **degrades beyond the training window** (2018–2020), underscoring the limits of basic trend models in a dynamic ecological system.

---

## 2) Evidence From Analyses

### 2.1 Scatter/Spatial perspective
- Scatter and map-style views show **dense clusters** around North America and Europe’s high-traffic airports (East Coast, Midwest, West Coast; UK/France/Germany; major US hubs such as NY, DC, FL, TX, LA, SF, SEA).  
- Interpretation: **air-traffic density + proximity to water/estuaries** jointly explain much of the spatial pattern.

### 2.2 Heatmap (regional hotspots)
- Heat concentrations align with **busy hubs and migration flyways**. Lack of hotspots over oceans and sparsely trafficked interiors supports the **airport-proximity** mechanism.

### 2.3 Speed histogram
- Distribution peaks near **140–160 kt** and tapers at cruise speeds; very few events > **300 kt**.  
- Practical implication: **terminal-area mitigation** (radar/monitoring/habitat management) offers the largest safety return.

---

## 3) Statistical Tests (α = 0.05)
- **Height–Speed relationship:** correlation is **statistically significant**, supporting expected flight dynamics.  
- **Two-sample comparison of speed** (approach vs landing-roll): **significant difference**; speed characteristics differ across the two terminal phases, consistent with differing risk exposure.  
- **Damage by phase:** a phase-group comparison shows **significant variation in damage severity**, with **approach** emerging as the most sensitive period.  
> Together, these results justify focusing modeling and mitigation on **phase-of-flight**, **speed**, and **airport-proximity/environmental** variables.

---

## 4) Predictive Modeling (trend baseline)
- **Setup:** simple linear regression on **AWP FAA region** annual counts (1990–2015); produce predictions for **2016–2017**, then extrapolate **2018–2020**.  
- **In-window fit:** captures broad trend and provides a **reasonable short-horizon forecast** for 2016–2017 when migration and traffic conditions are similar.  
- **Out-of-window behavior:** accuracy **drops** in 2018–2020, indicating **unmodeled external factors** (traffic changes, reporting shifts, ecology/weather).  
- **Implication:** use linear trend as an **illustrative baseline only**; operational planning should rely on richer models that incorporate **seasonality, airport-level traffic, habitat/weather, and species** signals.

---

## 5) Operational Implications
- Prioritize **airport-adjacent mitigation** (habitat management near runways, adaptive lighting/sound deterrents, real-time radar-based bird tracking).  
- Focus procedures on **approach/landing windows** where risk and damage concentrate.  
- For planning, deploy **seasonal playbooks** aligned with regional migration calendars.  
- For analytics, evolve toward **multi-factor models** (time series with seasonality + exogenous drivers) and site-level risk scoring.


### Summary
**Bird-strike risk concentrates at large, coastal, migration-adjacent airports—especially during approach and landing—peaking at 140–160 kt; linear trends explain short-term movement but fail farther out, motivating targeted, season-aware mitigation and richer predictive models.**
