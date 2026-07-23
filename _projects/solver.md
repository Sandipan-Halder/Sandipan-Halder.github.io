---
layout: post
title: "1D-Stellar-Hydrodynamics"
tagline: "A finite-volume fluid dynamics numerical solver configured in Python to compute 1D mass conservation profiles and trace shocks along circumstellar boundaries."
badge: "Python / Finite-Volume"
---

## 1. Governing Fluid Physics
This codebase solves standard mass continuity equations across moving stellar wind envelopes.

```python
# Core mass integration sweep
def update_density(rho, velocity, dt, dr):
    return rho - (dt / dr) * (rho * velocity)
```
