---
description: ''
---
### $p$ and $s$ polarization in optics

In optics, $p$ or $s$ polarization is defined relative to the plane of incidence (spanned by the incoming $k$ and the surface normal). 

$p$ (parallel) denotes electric field component parallel to the plane of incidence (a.k.a. TM).
$s$ (senkrecht/perpendicular) denotes electric field component perpendicular to the plane of incidence (a.k.a. TE).

Note: They are also sometimes called $\pi$ and $\sigma$, which are simply Greek designations for $p$ and $s$.

Example: 

![[example_s_p_polarization.png]]


### $\pi$ and  $\sigma^+$/$\sigma^-$ polarization in atomic physics

##### For absorption

In atom-light interaction, a static B-field defines the quantization axis (say $z$). The $\sigma^\pm/\pi$ polarization of the light is defined relative to the **quantization axis**.

$\sigma^+$ polarization refere to the electric field's spherical component $E_{+1}$, which drives $\Delta m=+1$ transition in the atom.
$\sigma^-$ polarization refers to the field's spherical component $E_{-1}$, which drives $\Delta m=-1$ transition.
$\pi$ polarization refers to field component $E_{0}$ (i.e. $\mathbf{E}\parallel \hat{z}$), which drives $\Delta m=0$ transition.

Note:  The labels $\sigma^\pm/\pi$ refer to the polarization components of the light, but they are also used to label transitions they drive in the atom because of the one-to-one correspondence with $\Delta m$. So when people say: “This is a $\sigma^+$ transition”, what they really mean is: “This transition is driven by $\sigma^+$  polarized light and therefore has $\Delta m = +1$.”

For plane wave, $\mathbf{k}\perp \mathbf{E}$, therefore:

- If $\mathbf{k}\parallel \hat{z}$, only $\sigma^\pm$ polarization (and transition) are possible (no $\pi$).  
- If $\mathbf{k}\perp \hat{z}$, $\pi$ corresponds to $\mathbf{E}\parallel \hat{z}$, and $\mathbf{E}\perp \hat{z}$ is a **linear** polarization that is an equal superposition of $\sigma^+$ and $\sigma^-$.

##### For spontaneous emission of photons

Considering photons emitted by an atom, the polarization of the photons depend on transitions in the atom and observation directions:

| Transition   | Observe along (z) | Observe ⟂ (z)   |
| ------------ | ----------------- | --------------- |
| Δm = 0 (π)   | No light          | Linear, **‖ B** |
| Δm = +1 (σ⁺) | Circular (σ⁺)     | Linear, ⟂ B     |
| Δm = −1 (σ⁻) | Circular (σ⁻)     | Linear, ⟂ B     |
 
 Physical intuition for this:
- Dipoles never radiate along their oscillation axis.
- π → dipole oscillating along B → looks linear when viewed from side.
- σ → dipole rotating in xy-plane → looks circular when viewed along B.


Note: in any cases, $\sigma$ (without plus or minus in the notation) means linearly polarized light.
