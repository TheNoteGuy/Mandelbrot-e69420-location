# 1e-69420 end minibrot — results

## Final minibrot

| | |
|---|---|
| Period P | **700,679** |
| \|size\| | **3.386203e-69421** = 0.3386 × final half-width (window 0.25–0.35) |
| arg(size) | **−0.162256 rad (−9.30°)**: lies almost horizontally, tail pointing left |
| Final half-width | exactly 1e-69420 |
| Nucleus | `locations/final_hw_1e-69420.txt`: 69,500 decimals per coordinate,`set MB_…` format |

## Verification (full report: `verification_raw.txt`)

| Check | Result |
|---|---|
| Residual \|z_P(c)\| at 231,700 bits | 1e-34802.4 |
| Next Newton step \|z_P/z_P′\| at 231,700 bits | 1e-69512.6 = 1e-92 × \|size\| (stop rule: < 1e-30 × \|size\|) |
| Period re-check | Direct full-precision ball method, disk radius 1e-3·\|size\| around c. The first k whose ball image contains 0 is k = 700,679 = P. For every k < P, \|z_k\| ≥ 1e34712 × ball radius. |
| Size stability | 289,625-bit orbit with 256-bit accumulators gives log10\|size\| = −69420.470287254 and arg = −0.162255941. Differences from the 231,700-bit pass: 0 (to 1e-9) and 3.4e-13 rad. |

## Chain (`chain.csv`: all 5,145 minibrots with depth, period, |size| and rotation)

| stage | period | depth (−log10\|size\|) | rotation |
|---:|---:|---:|---:|
| 0 (start) | 184,886 | 2,021.15 | 75.8° |
| 500 | 236,857 | 8,695.49 | −61.1° |
| 1000 | 286,705 | 15,279.25 | −83.7° |
| 1500 | 336,785 | 21,879.66 | −22.0° |
| 2000 | 386,908 | 28,474.94 | −85.4° |
| 2500 | 437,719 | 35,125.79 | −131.0° |
| 3000 | 488,188 | 41,756.65 | −77.1° |
| 3500 | 537,847 | 48,196.17 | −11.2° |
| 4000 | 587,053 | 54,692.41 | 77.9° |
| 4500 | 637,586 | 61,122.00 | −176.1° |
| 5000 | 686,622 | 67,590.61 | 79.1° |
| 5143 | 700,558 | 69,406.73 | 81.3° |
| **5144 (final)** | **700,679** | **69,420.47** | **−9.3°** |

## Test renders

- `preview_final.png`: the minibrot fills the frame nicely. The tail tip is about 0.68 half-widths left of centre and the cusp about 0.09 to the right.
- `preview_up4.png`: the minibrot is a small mark at the centre.
- `preview_up16.png`: the minibrot is about 0.003 px across, so only centred escape bands are visible.
