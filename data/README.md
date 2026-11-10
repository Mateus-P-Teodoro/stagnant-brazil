# Data Sources & Access

This folder does not contain raw `.csv` or `.xlsx` files. To ensure reproducibility and to avoid large file hosting, all macroeconomic time series are queried and downloaded automatically at runtime using the [`ipeadatar` package API](https://github.com/ipea/ipeadatar).

Below is the documentation and the original official sources for the datasets manipulated in this research:

### 1. Demographic Dependency Ratio (DDR)
* **API Series Code:** `ADH12_RAZDEP`
* **Original Source:** IBGE (Demographic Census & PNAD) via Atlas of Human Development.
* **Description:** Proportion of the inactive population (0-14 and 65+ years) relative to the potentially productive population (15 to 64 years).
* **Reference Link:** [Ipeadata Metadata - ADH12_RAZDEP](http://www.ipeadata.gov.br/ExibeSerie.aspx?serid=62006)

### 2. Brazilian Labor Productivity
Calculated in the script as the ratio between Real GDP and Total Employed Persons.
* **Real GDP (Numerator):** 
  * API Series Code: `SCN10_PIBP10` 
  * Source: IBGE - System of National Accounts (SCN).
  * Reference Link: [Ipeadata Metadata - SCN10_PIBP10](http://www.ipeadata.gov.br/ExibeSerie.aspx?serid=63510)
* **Employed Persons (Denominator):** 
  * API Series Code: `PAN_PO` 
  * Source: IBGE - Continuous National Household Sample Survey (PNAD Contínua).
  * Reference Link: [Ipeadata Metadata - PAN_PO](http://www.ipeadata.gov.br/ExibeSerie.aspx?serid=1626012678)

### 3. Global Benchmarks
* **Original Source:** World Bank Open Data (World Development Indicators).
* **Description:** GDP per person employed for the control group (Vietnam, Poland, South Korea, Chile).
* **Reference Link:** [World Bank Data Portal](https://data.worldbank.org/indicator/SL.GDP.PCAP.EM.KD)
