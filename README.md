# India Agricultural Census 2015-16 — District-level Scraped Data

This repository contains district-level data from India's Agricultural Census 2015-16, scraped from the Government of India's official Agricultural Census portal at [agcensus.da.gov.in](https://agcensus.da.gov.in). The data covers operational landholdings across Indian states and union territories, broken down by social group, farm size, and tenure type.

All files are in standard CSV format and can be opened in Excel, Google Sheets, R, Python (pandas), or any data tool.

---

## What is an operational holding?

The Agricultural Census is conducted every five years by the Department of Agriculture & Farmers Welfare, Government of India. It is the most comprehensive source of data on agricultural landholdings in India — covering how many farms exist, who owns or operates them, how large they are, and which social groups they belong to.

An operational holding is a unit of land used wholly or partly for agricultural production and operated by one person — either alone or with others — regardless of the title, legal form, size, or location of the land. Importantly, it is not the same as ownership of the land: a tenant farmer operating rented land counts as an operational holding.

The 2015-16 census is the most recent one for which district-level data is publicly available. I hope to make data for the last 3 agricultural censuses, conducted in  available soon

---

## Limitations

Please read these carefully before using the data in research or analysis.

**1. The data reflects what the portal reports — not independently verified**
This dataset is a direct scrape of the official portal. Any errors, inconsistencies, or revisions in the source data are carried over. The Agricultural Census itself is known to have some underreporting, particularly for marginal and small holdings in remote areas.

**2. `ALL SOCIAL GROUPS` is excluded**
The row representing the total across all social groups has been intentionally left out. It is a simple sum of SC + ST + Others + Institutional and can be computed from the existing rows.

**3. Spelling follows the government portal**
State and district names match exactly how they appear in the website's dropdown menus. This means some spellings differ from standard usage — for example, the portal uses `TELENGANA` (not Telangana), `CHATTISGARH` (not Chhattisgarh), and short forms like `D & N HAVELI` for Dadra and Nagar Haveli. Do not modify these spellings if merging with other portal-derived data.

**4. Jammu & Kashmir reflects pre-2019 boundaries**
The 2015-16 census was conducted when J&K was a full state. It was bifurcated into two Union Territories (J&K and Ladakh) in 2019. The data here covers the undivided state.

**5. Gender breakdown not included**
This dataset only covers `TOTAL` (male + female combined). The portal does have separate male/female breakdowns which have not been scraped here. The reason is that I plan to make data for prior years available soon, which in fact does not have the male/female breakdowns.

---

## Source

- **Portal:** [https://agcensus.da.gov.in](https://agcensus.da.gov.in)
- **Table:** "Number & Area of Operational Holdings by Size Group" under (District Summary)
- **Published by:** Department of Agriculture & Farmers Welfare, Government of India

---

## Feedback

This repository is maintained by [Pranav Aggarwal](https://x.com/pranav_so). I am very happy to get feedback on the project --- comments, suggestions for improvement, errors in data, and so on. If you found this data helpful, please share it with others to whom it might also be of use.  
