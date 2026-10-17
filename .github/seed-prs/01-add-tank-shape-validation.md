---
title: "feat(tank-sizer): validate tank shape options"
labels: ["enhancement"]
---

Adds a `tank_shape` parameter to `OutWestSepticTankSizer.__init__` with options: `round`, `low_profile`, `two_compartment`. The script validates the value and raises `ValueError` for invalid shapes.

**Why**

Different site constraints call for different tank shapes. Low-profile for shallow sites, round for typical, two-compartment for new installations per TCEQ.

**Diff highlights**

```python
ALLOWED_SHAPES = ("round", "low_profile", "two_compartment")

def __init__(self, gpd_per_bedroom=150, tank_shape="two_compartment"):
    if tank_shape not in self.ALLOWED_SHAPES:
        raise ValueError(f"tank_shape must be one of {self.ALLOWED_SHAPES}")
    ...
```

**Verified**

```bash
python scripts/outwestseptic_tank_sizer.py 3
# works
python -c "from outwestseptic_tank_sizer import OutWestSepticTankSizer; OutWestSepticTankSizer(tank_shape='invalid')"
# raises ValueError
```

---

*Out West Septic — TCEQ OSSF Installer I — OS0041298*