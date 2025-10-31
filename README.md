# Wildlife Strike Analytics
Analyze wildlife (bird) strikes to understand safety risk, financial costs, and operational disruptions, and to uncover trends and drivers across flight phase, aircraft type, and location.


## Objectives
- Track **trends** in wildlife/bird strikes over time (national and by region).
- Identify **drivers**: flight phase, aircraft type, airport/state/region, seasonality.
- Estimate **impact**: damage categories and proxy **cost** signals.
- Build simple **predictive models** to forecast near-term incidents and illustrate limitations of linear extrapolation.

## Data
- **Source:** FAA Wildlife Strike dataset (bird strikes focused).  
- **Scope:** year, month, FAA region, state/airport, aircraft type, phase of flight, species, damage, cost fields.  
- **Cleaning:** normalize categorical labels, handle missing values, and remove obvious outliers; keep only complete records for key analyses.  
- **Unit of analysis:** one record = one reported strike.

**▶ Notebook:** `Bird-Strike-Safety-and-Costs.ipynb`  
**▶ Report:** `reports.md`
