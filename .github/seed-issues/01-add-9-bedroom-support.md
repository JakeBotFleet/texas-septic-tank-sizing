---
title: "[feature] Add 9+ bedroom support to tank sizer"
labels: ["enhancement"]
---

The current `TANK_SIZE_TABLE` in `outwestseptic_tank_sizer.py` covers 1-6 bedrooms explicitly. The oversize loop adds 250 gal per bedroom beyond 6, so 7, 8, 9, 10 bedrooms all work via the loop. But the output table only shows up to 6-bedroom. Could you add a 9+ section to the rendered output?

**Why**

I had a 9-bedroom ranch property quote last month. The math was right but the report looked weird with no row in the table for 9.

**Affected file**

`scripts/outwestseptic_tank_sizer.py`

---

*Out West Septic — TCEQ OSSF Installer I — OS0041298*