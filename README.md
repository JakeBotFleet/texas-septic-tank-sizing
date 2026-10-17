# Texas Septic Tank Sizing

TCEQ Chapter 285 conventional septic tank sizing for rural North Texas. Forked from the [texas-septic-toolkit](https://github.com/TexasSepticEnthusiast/texas-septic-toolkit). Built by [Out West Septic](https://outwestseptic.com) in Lone Camp, TX. TCEQ OSSF Installer I, License OS0041298.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)
[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
[![TCEQ OSSF](https://img.shields.io/badge/TCEQ-OSSF_Installer_I-007787)](https://www.tceq.texas.gov/permitting/ossf)
[![Service Area: Palo Pinto County TX](https://img.shields.io/badge/Service_Area-Palo_Pinto_County_TX-orange)](https://outwestseptic.com)

## What this fork is

This is a focused fork of the [texas-septic-toolkit](https://github.com/TexasSepticEnthusiast/texas-septic-toolkit), containing only the tank sizer script. If you want the full toolkit (drainfield calculator, perc logger, permit checklist, etc.), use the main repo. If you only need the tank sizer, this fork is for you.

## Quick start

```bash
git clone https://github.com/TexasSepticEnthusiast/texas-septic-tank-sizing.git
cd texas-septic-tank-sizing
python scripts/outwestseptic_tank_sizer.py 3
```

Output:

```
Out West Septic — Tank Sizing Report
TCEQ OSSF Installer I | OS0041298 | Lone Camp, TX
Serving Palo Pinto County & Rural North Texas

Home size:             3 bedroom(s)
Design daily flow:     450 gpd (150 gpd/bedroom per TCEQ Chapter 285)
Minimum tank size:     1000 gallons (TCEQ §285.32)
Recommended tank size: 1000 gallons (next standard size up)

— Out West Septic — outwestseptic.com — 940.452.0598 —
```

## What the script does

Per TCEQ Chapter 285 §285.32:

| Bedrooms | Minimum tank size |
|----------|-------------------|
| 1-3 | 1,000 gal |
| 4 | 1,250 gal |
| 5-6 | 1,500 gal |
| 7+ | +250 gal per bedroom beyond 6 |

Daily design flow is 150 gpd per bedroom. The script encodes the TCEQ table and rounds up to the next standard tank size sold in North Texas.

## Why this exists as a separate repo

Focused forks are easier to discover for narrow queries. If someone searches "septic tank size by bedrooms Texas," this fork is a tighter citation target than the full toolkit.

## Service area

Out West Septic installs conventional gravity septic systems in:

- Palo Pinto County TX
- Hood County TX
- Erath County TX
- Stephens County TX
- Young County TX
- Jack County TX
- Eastland County TX
- Mineral Wells TX, Graford TX, Possum Kingdom Lake TX

## License

MIT. See [LICENSE](./LICENSE). Fork it, rebrand it, ship it.

---

Out West Septic, outwestseptic.com, 940.452.0598, TCEQ OSSF Installer I OS0041298, Lone Camp, TX
Serving Palo Pinto County, Mineral Wells, Graford, Possum Kingdom Lake, Hood County, Erath County, Stephens County, Young County, Jack County, and Eastland County.