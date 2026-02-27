---
description: ''
---
References:
- For solving non-homogeneous linear ODE: see [Exponential response formula](https://en.wikipedia.org/wiki/Exponential_response_formula)
- Detailed derivation of damped oscillation: see [Link](https://beltoforion.de/en/harmonic_oscillator/) or [this pdf](Damped_Harmonic_Oscillator.pdf)
- Confirmation of the content of this note: [this pdf](lecture2-driven-oscillators.pdf)


### Harmonic oscillation

Force: $F=-kx$

Equation of motion: $m\ddot{x}=F \Longrightarrow \ddot{x}+\omega_{0}^{2}x=0$, where $\omega_{0}\equiv \sqrt{\frac{k}{m}}$.

Solution in real domain: 
$$
x(t)=A\cos{(\omega_0 t+\phi)}
$$ 
Energy: $E=\frac{1}{2}m\omega_{0}^{2}A^{2}=\frac{1}{2}kA^2$, meaning it depends on the mass, oscillation frequency, and oscillation amplitude.


### Damped oscillation

Force: $F=-kx-bv$, where $b$ is called the viscous damping coefficient.

Equation of motion: $m\ddot{x}=F \Longrightarrow \ddot{x}+\gamma \dot{x}+\omega_{0}^{2}x=0$, where $\gamma \equiv \frac{b}{m}$.

Solution: 
- Overdamped case ($\gamma \gt 2\omega_0$):
$$
x(t)=e^{-\frac{\gamma}{2}t}(c_{1}e^{\omega_{\gamma}t} + c_{2}e^{-\omega_{\gamma}t})
$$
where $\omega_{\gamma}\equiv \sqrt{(\frac{\gamma}{2})^{2}-\omega_{0}^{2}}$.
- Critically damped case ($\gamma = 2\omega_0$):
$$
x(t)=e^{-\frac{\gamma}{2}t}(c_1+c_2t)
$$
- Underdamped case ($\gamma \lt 2\omega_0$):
$$
x(t)=e^{-\frac{\gamma}{2}t}A\cos(\omega't+\varphi)
$$
where $\omega'\equiv\sqrt{\omega_{0}^{2}-(\frac{\gamma}{2})^{2}}$.

### Driven oscillation without damping

Force: $F=-kx+F_0\cos(\omega t)$, here assuming a periodic driving force.

Equation of motion: $m\ddot{x}=F \Longrightarrow \ddot{x}+\omega_{0}^{2}x=\frac{F_{0}}{m}\cos{\omega t}$

Solution:
$$
x(t)=A\cos{(\omega_0 t+\phi)} - \frac{F_{0}/m}{\omega^{2}-\omega_0^2}\cos\omega t
$$
The solution for initial conditions $x(0)=\dot{x}(0)=0$ is

$$
\begin{aligned}
x(t)&=-\frac{F_{0}/m}{\omega^{2}-\omega_{0}^{2}}(\cos\omega t-\cos\omega_{0}t)\\
&=\frac{2F_{0}/m}{\omega^{2}-\omega_{0}^{2}}\sin\left(\frac{\omega-\omega_0}{2} t\right)\sin \left(\frac{\omega+\omega_0}{2} t\right)
\end{aligned}
$$

If $\omega\approx\omega_0$, there is $\omega^{2}-\omega_{0}^{2}\approx 2\omega_0(\omega-\omega_{0})$ and $\sin \frac{\omega-\omega_0}{2} t\approx\frac{\omega-\omega_0}{2} t$, then
$$
x(t)=\frac{F_{0}}{2m\omega_0}t\sin\omega_0t
$$
meaning the amplitude of the oscillation keeps increasing over time, and (for the specified initial conditions) the phase delay relative to the driving force is $\frac{\pi}{2}$, as $\sin\omega_{0}t=\cos\left( \omega_{0} t-\frac{\pi}{2} \right)$: **resonance**.

If $\omega\gg\omega_0$, then
$$
x(t)=\frac{2F_{0}}{m\omega^2}\sin^2{\frac{\omega}{2}}t=\frac{F_0}{m\omega^2}(1-\cos\omega t)
$$
meaning the oscillation amplitude $\frac{F_0}{m\omega^2}$ is very small, and the phase delay relative to the driving force is $\pi$.

### Driven oscillation with damping

Force: $F=-kx-bv+F_0\cos(\omega t)$

Equation of motion: $m\ddot{x}=F \Longrightarrow \ddot{x}+\gamma \dot{x} + \omega_{0}^{2}x=\frac{F_{0}}{m}\cos{\omega t}$.

Solution: 
$$
\begin{aligned}
x(t)&=\mathrm{G.S.}+\frac{F_{0}}{m}\frac{(\omega_{0}^{2}-\omega^{2})\cos{\omega t}+\gamma\omega\sin{\omega t}}{(\omega_{0}^{2}-\omega^{2})^{2}+\gamma^{2}\omega^{2}} \\
&=\mathrm{G.S.}+\frac{F_{0}/m}{\sqrt{(\omega_{0}^{2}-\omega^{2})^{2}+\gamma^{2}\omega^{2}}}\cos(\omega t-\varphi)\qquad\textrm{where }\tan{\varphi=\frac{\gamma\omega}{\omega_{0}^{2}-\omega^{2}}}
\end{aligned}
$$
where $\mathrm{G.S.}$ stands for the general solution in [[#Damped oscillation]] given above, which will decay to infinitesimal and is thus often left out, if the steady state is considered.

Therefore, the steady-state solution
$$
\begin{aligned}
x(t)&=U\cos{\omega t}+V\sin{\omega t}\\
&=\frac{F_{0}}{m}\frac{(\omega_{0}^{2}-\omega^{2})}{(\omega_{0}^{2}-\omega^{2})^{2}+\gamma^{2}\omega^{2}}\cos{\omega t}+\frac{F_{0}}{m}\frac{\gamma\omega}{(\omega_{0}^{2}-\omega^{2})^{2}+\gamma^{2}\omega^{2}}\sin{\omega t}
\end{aligned}
$$

contains the component that is in-phase with the force $F_0\cos(\omega t)$ and the quadrature component that has a phase delay of π/2 with respect to the force. 

The change of $U$, $V$ and $\varphi$ as driven frequency $\omega$ sweeps through resonance $\omega_{0}$:

![[driven_oscillation.png]]

The power absorbed by the oscillation equals the power done by the driving force:
$$
P=Fv=F_0\cos\omega t\times\dot{x}(t)=-F_0U\omega\sin\omega t\cos\omega t+F_0V\omega\cos^2\omega t
$$
The average absorption power is
$$
\overline{P}=\frac{F_0V\omega}{2}
$$
meaning the absorption of energy arises only from the quadrature component 
$$
V=\frac{F_{0}}{m}\frac{\gamma\omega}{(\omega_{0}^{2}-\omega^{2})^{2}+\gamma^{2}\omega^{2}}\approx\frac{F_{0}}{2m\omega}\frac{\gamma/2}{(\omega-\omega_0)^2+(\gamma/2)^2}
$$
which is a Lorentzian line shape function.

At resonance $\omega=\omega_0$, the steady state is: 
$$
x(t)=\frac{F_0}{m\gamma\omega}\sin\omega t
$$
The power absorbed by the oscillation equals the power done by the driving force: 
$$
P=Fv=F_0\cos\omega t\times\frac{F_0}{m\gamma}\cos{\omega t}=\frac{F_0^2}{m\gamma}\cos^{2}{\omega}t
$$
which also equals the power dissipated by the damping force $F_d=-bv$:
$$
P =bv^2=m\gamma\times\frac{F_0^2}{m^2\gamma^2}\cos^2\omega t=\frac{F_0^2}{m\gamma}\cos^{2}{\omega}t
$$
meaning the driving force essentially overcomes the damping force all the time (actually driving force equals damping force) so that $x(t)$ is a harmonic oscillation with $\ddot{x}+\omega^{2}x=0$. The average absorption power is $\overline{P}=\frac{F_0^2}{2m\gamma}$.

### Application

[[Lorentz-Drude model ]]

