# Platonic Solids — Oscillating Peaks Animation
## Convex ↔ Concave morphing via Spherical Harmonics

**Reference:** [Chebfun — Spherical Harmonics §6](https://www.chebfun.org/examples/sphere/SphericalHarmonics.html)

---

### Animation principle

The radial deformation amplitude $\alpha$ is swept through a full cosine cycle:

$$\alpha(t) = \alpha_{\max} \cdot \cos\!\left(\frac{2\pi\,k}{N_\text{frames}}\right), \quad k = 0,1,\dots,N_\text{frames}-1$$

| Phase | $\alpha$ | Shape |
|---|---|---|
| $k=0$ | $+\alpha_{\max}$ | **Fully convex** — normal solid |
| $k=N/4$ | $0$ | **Unit sphere** — no deformation |
| $k=N/2$ | $-\alpha_{\max}$ | **Fully concave** — inverted solid |
| $k=3N/4$ | $0$ | **Unit sphere** again |

The surface colour (driven by the static $\hat{Y}_\ell^m$ field) stays fixed —
only the geometry oscillates, making the convex/concave transition visually clear.

> **Controls:** ▶ Play · ⏸ Pause · drag the frame slider below each figure
