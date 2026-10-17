# Texas Septic Tank Sizing Reference

> **Quick answer:** Per TCEQ Chapter 285 §285.32, the minimum septic tank size is determined by bedroom count: 1–3 bedrooms needs 1,000 gal, 4 needs 1,250, 5–6 needs 1,500, and 7+ adds 250 gal per bedroom beyond 6. Daily design flow is 150 gpd per bedroom.

## The minimum size table

| Bedrooms | Minimum liquid capacity |
|----------|------------------------|
| 1 | 1,000 gal |
| 2 | 1,000 gal |
| 3 | 1,000 gal |
| 4 | 1,250 gal |
| 5 | 1,500 gal |
| 6 | 1,500 gal |
| 7 | 1,750 gal |
| 8 | 2,000 gal |
| 9 | 2,250 gal |
| 10 | 2,500 gal |

## How the script works

The `outwestseptic_tank_sizer.py` script encodes the TCEQ table and rounds up to the nearest standard tank size sold in North Texas:

- 1,000 / 1,250 / 1,500 / 1,750 / 2,000 / 2,500 / 3,000 gal

## Source

- TCEQ Chapter 285 §285.32 design criteria: https://www.tceq.texas.gov/permitting/ossf

**last_verified:** 2026-10-17

---

*Out West Septic — outwestseptic.com — TCEQ OSSF Installer I OS0041298 — Lone Camp, TX — 940.452.0598*