# Tube Bender Layout Calculator

A single-page tool for laying out **hand-bent rigid tubing** using the **Swagelok measure-bend method** (per *Swagelok Hand Tube Bender Manual, MS-13-43*). Built for the **MSU Rocketry Lab (RTS / LOX-RP1 vehicle assembly)**.

👉 **Live tool:** https://noureldin0007.github.io/tube-bender-calculator/

No install — it's one self-contained `index.html`. Open it in any browser.

## What it does

Given the shape of a tube you want to bend, it tells you:
- the **straight cut length** to start from,
- **where to mark each bend** (the vertex position, measured from end A), and
- the bend angles, turn directions, and adjustments.

### Features
- **Shapes:** 90°/single bend, S-offset (incl. **90° square-S**), U-bend, free-hand **sketch → refit**, and a multi-bend **table** entry.
- **Edit on the diagram:** click any orange number to set a leg length, any red number to set a bend angle.
- **Swagelok-correct math:** uses the published adjustment (gain) table from MS-13-43 p.23, with a geometric fallback (`2·R·tan(θ/2) − R·θ`) for non-tabulated angles. Verified against the manual's worked example (¼" tube, 9/16 R, two 90° bends, legs 3/2.5/3 → 7‑7/8" cut, marks 3" and 5‑3/16").
- **Required straight L** auto-filled per tube OD so the tube can bottom in the fitting and the ferrules grip.
- **Springback compensation** (1–3° per MS-13-43 p.19) added to the printed bend targets.
- **Flaring support:** 37° JIC/AN or 45° SAE ends — sets the flare-tool clamp length, adds flare takeup to the raw cut, and prints the *"put the nut on before flaring"* reminder.
- **Outputs:** copy-able cut list, print view, and a fully-dimensioned **SVG export**.
- Inch (with nearest 1/64") and mm units.

## Reference

- Swagelok *Hand Tube Bender Manual* — MS-13-43
- Swagelok *Gaugeable Tube Fittings* — MS-01-140

## Notes

Dimensions are a layout aid — always test-fit dry before final assembly, and confirm bend radius and tube wall are within the bender's rated range. Adjustment values match the Swagelok hand benders (1/8–1/2" and 3–12 mm dies).

---
*Internal lab tool. Not affiliated with or endorsed by Swagelok Company.*
