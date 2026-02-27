*Refs:
电动力学，第三版，郭硕鸿*

### Scalar and vector potential

The Maxwell's equations for electromagnetic field in vacuum are:
$$\begin{aligned}
&\nabla\times\boldsymbol{E}=-\frac{\partial\boldsymbol{B}}{\partial{t}}\quad(1)\\[0.5em]
&\nabla\times\boldsymbol{H}=\frac{\partial\boldsymbol{D}}{\partial{t}}+\boldsymbol{J}\quad(2)\\[0.5em]
&\nabla\cdot\boldsymbol{D}=\rho\quad(3)\\[0.5em]
&\nabla\cdot\boldsymbol{B}=0\quad(4)\\[0.5em]
&(\boldsymbol{D}=\varepsilon_0\boldsymbol{E},\ \boldsymbol{B}=\mu_0\boldsymbol{H})
\end{aligned}$$
From Eq. (4), $\boldsymbol B$ is generally a field without sources, so a vector potential $\boldsymbol{A}$ can be introduced such that $$\boxed{\boldsymbol B=\nabla\times\boldsymbol A}\quad(5)$$
From Eq. (1) and (3), $\boldsymbol{E}$ is generally a field with both curl and source (different from a static electric field which has no curl and can thus be described with a scalar potential). Inserting $\boldsymbol B=\nabla\times\boldsymbol A$ into Eq. (1) yields
$$\nabla\times(\boldsymbol{E}+\frac{\partial\boldsymbol{A}}{\partial{t}})=0$$
meaning $\boldsymbol{E}+\frac{\partial\boldsymbol{A}}{\partial{t}}$ is a field without curl, so a scalar potential $\varphi$ can be introduced such that $\boldsymbol{E}+\frac{\partial\boldsymbol{A}}{\partial{t}}=-\nabla{\varphi}$:
$$\boxed{\boldsymbol{E}=-\nabla{\varphi}-\frac{\partial\boldsymbol{A}}{\partial{t}}}$$
### Gauge transformation

The correspondence between $\boldsymbol{A},~\varphi$ and $\boldsymbol{B},~\boldsymbol{E}$ is not one-to-one. Performing the following transformation (gauge transformation) to $\boldsymbol{A},~\varphi$:
$$\begin{aligned}\boldsymbol{A}\rightarrow \boldsymbol{A'}=\boldsymbol{A}+\nabla\psi\\[0.5em]
\varphi\rightarrow \varphi'=\varphi-\frac{\partial\psi}{\partial{t}}
\end{aligned}$$
where $\psi$ is an arbitrary scalar function, then it is easy to prove that $(\boldsymbol{A'},~\varphi')$ and $\boldsymbol{A},~\varphi$ describe the same electromagnetic field.

### Gauge invariance

One combination of $(\boldsymbol{A},~\varphi)$ is called one gauge. Since the gauge transformation does not change the $\boldsymbol{B},~\boldsymbol{E}$ field, the law of physics does not depend on the choice of specific gauge to describe the electromagnetic field. 

The invariance of physical observables and law of physics under gauge transformation is called gauge invariance.

### Two useful gauges
The reason that there is freedom in the choice of gauge is that only the curl of $\boldsymbol A$ is given in its definition Eq. (5), but not the divergence. Since in principle there is no any restriction on $\nabla\cdot\boldsymbol{A}$, it can be taken as any value for convenience. One setting of $\nabla\cdot\boldsymbol{A}$ corresponds to one gauge. The two mostly used gauges are:

##### Coulomb gauge 
$$\nabla\cdot\boldsymbol{A}=0$$
##### Lorentz gauge
$$\nabla\cdot\boldsymbol{A}+\frac{1}{c^{2}}\frac{\partial\varphi}{\partial{t}}=0$$
or in Lorentz invariant form as $\partial_uA^u=\frac{\partial{A^u}}{\partial{x^u}}=0$.

Using this gauge, the equation for $\boldsymbol{A},~\varphi$ can be derived from Maxwell's equations as **the d'Alembert equation**:
$$\begin{aligned}
\nabla^2\boldsymbol{A}-\frac{1}{c^{2}}\frac{\partial^2\boldsymbol{A}}{\partial{t^2}}=-\mu_0\boldsymbol{J}\\[0.5em]
\nabla^2\varphi-\frac{1}{c^{2}}\frac{\partial^2\varphi}{\partial{t^2}}=-\frac{\rho}{\varepsilon_0}
\end{aligned}$$
or $\Box A^u=-\mu_0J^u$, where $\Box\equiv\partial^u\partial_u=\nabla^2-\frac{1}{c^{2}}\frac{\partial^2}{\partial{t^2}}$ and $J^u=(c\rho,\boldsymbol{J})$.