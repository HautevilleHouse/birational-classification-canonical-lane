# Extraction Spec

Framework: `birational_classification`

Required constants:

- `kappa_birational`
- `sigma_model`
- `kappa_compact`
- `rho_rigidity`
- `birational_lock`
- `eps_coh`
- stitch key `sigma_star_can`

All constants are extracted from explicit formulas in `artifacts/constants_extraction_inputs.json`, promoted into the registry and stitch files, then consumed by the closure guard.
