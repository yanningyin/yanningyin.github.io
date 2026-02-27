Ref: [Wikipedia](https://en.wikipedia.org/wiki/Dispersion_relation)

### Dispersion relation

Dispersion is the phenomenon in which the phase velocity of a wave depends on its frequency.

The dispersion relation can be expressed as $f(\lambda)$ or $\omega(k)$. Dispersion occurs when sinusoidal waves of different wavelengths have different propagation velocities: $v=v(\lambda)$. The velocity relates to the wavelength and frequency by: $v(\lambda)=\lambda f(\lambda)$. Since $\omega=2\pi f$ and $k=2\pi/\lambda$, this relation can also be expressed as $v(k)=\omega(k)/k$ (phase velocity).


### (Ordinary)Refractive index

The ratio between the speed of light $c$ and the phase velocity $v_p$ is the **refractive index**: $$n(\omega)=\frac{c}{v_p(\omega)}=\frac{ck(\omega)}{\omega}$$
In this way, we can obtain the relation between group velocity ($v_g=\partial \omega/\partial{k}$) and phase velocity. Writing $n= n(\omega)$, we have

$$\displaystyle k={\frac {1}{c}}\omega n(\omega )\implies dk={\frac {1}{c}}\left(n(\omega )+\omega {\frac {\partial }{\partial \omega }}n(\omega )\right)d\omega$$

We can then rearrange the above to obtain: $\displaystyle v_{g}={\frac {\partial w}{\partial k}}={\frac {c}{n+\omega {\frac {\partial n}{\partial \omega }}}}$
From this formula, we see that the group velocity is equal to the phase velocity only when the refractive index is independent of frequency $\textstyle \partial n/\partial \omega =0$. When this occurs, the medium is called non-dispersive, as opposed to [dispersive](https://en.wikipedia.org/wiki/Dispersion_(optics) "Dispersion (optics)"), where various properties of the medium depend on the frequency $\omega$.

### Complex refractive index

To incorporate the absorption when light passes through a medium, a complex refractive index can be defined as $\tilde{n}(\omega)=n+i\kappa$, where $n$ is the ordinary refractive index shown above, and $\kappa$ is called optical extinction coefficient.

Assuming a light with wave vector in vacuum $k_0$ propagates in a medium, the wave vector will become $\tilde{k}=\tilde{n}k_0$ and the expression for the light is
$$\boldsymbol{E}(x,t)=\mathrm{Re}[\boldsymbol{E}_0e^{i(\tilde{k}x-\omega{t})}]=\mathrm{Re}[\boldsymbol{E}_0e^{i[(n+i\kappa)k_0x-\omega{t}]}]=e^{-\kappa{k_0x}}\textrm{Re}[\boldsymbol{E}_0e^{i(nk_0x-\omega{t})}]$$

If we define $k\equiv nk_0$, then $k(\omega)$ represents the dispersion. We also see that $\kappa$ gives an exponential decay (absorption), as expected from the [[Beer–Lambert law]]. Since intensity is proportional to the square of the electric field, intensity will depend on the depth into the material as 
$${\displaystyle I(x)=I_{0}e^{-2\kappa k_0x}}$$
and thus the absorption coefficient is $\alpha = 2\kappa k_0$  and the penetration depth (the distance after which the intensity is reduced by a factor of 1/e) is $\delta_p = 1/\alpha$.

### Relation among $n$, $\varepsilon_r$ and $\chi$

From $c=\frac{1}{\sqrt{\mu_0\varepsilon_0}}$, $v_p=\frac{1}{\sqrt{\mu\varepsilon}}=\frac{1}{\sqrt{\mu_0\mu_r\varepsilon_0\varepsilon_r}}$ and $n=\frac{c}{v_p}$, we have $n=\sqrt{\mu_r\varepsilon_r}$, and its complex form also holds: $\tilde{n}=\sqrt{\tilde{\mu}_r\tilde{\varepsilon}_r}$.

Most naturally occurring materials are non-magnetic at optical frequencies, that is $\mu_r$ is very close to 1, therefore $n\approx \sqrt{\varepsilon_r}$ and $\tilde{n}\approx\sqrt{\tilde{\varepsilon}_r}$.

Relative permittivity $\varepsilon_r$ is directly related to electric susceptibility $\chi$ by $\varepsilon_r=1+\chi$. The complex electric susceptibility $\chi$ (and $n=\sqrt{\varepsilon_r}$) can be derived in, e.g., [[Lorentz-Drude model]] or [[Absorption and dispersion in QM]]. From $\tilde{n}$ we can know the dispersion and absorption of the wave when passing through the medium.
