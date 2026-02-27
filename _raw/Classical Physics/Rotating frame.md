---
description: ''
---

References:
[Wikipedia](https://en.wikipedia.org/wiki/Rotating_reference_frame)

### Rotating frame
A rotating frame is a special case of a non-inertial reference frame.

Note that when describing a system in different frames, the energies of the system are not necessarily the same. For example, a table at rest in the Earth's frame has zero kinetic energy, but when looking from the frame of the Sun, it can have non-zero kinetic energy due to the Earth's spin.

### Positions in two frames
Suppose a rotating frame $x'y'z'$ is rotating about the $z$ axis of an inertial frame $xyz$ with angular frequency $\boldsymbol\Omega=(0,0,\Omega)$, then the coordinates in the two frame are related by
$$
\begin{bmatrix}x'\\y'\end{bmatrix}=\begin{bmatrix}\cos\Omega{t} & \sin\Omega{t}\\-\sin\Omega{t} & \cos\Omega{t} \end{bmatrix}\begin{bmatrix}x\\y\end{bmatrix}
$$
### Time derivatives in two frames
Suppose $\hat{\boldsymbol{\imath}},\hat{\boldsymbol{\jmath}}$ are the basis vectors in the rotating frame, then their coordinates in the inertial frame are
$$
{\hat{\boldsymbol{\imath }}}(t)=(\cos\Omega{t},\sin\Omega{t}),\quad{\hat{\boldsymbol{\jmath }}}(t)=(-\sin\Omega{t},\cos\Omega{t})
$$
The time derivatives in the inertial frame are
$$
\frac{\mathrm{d}\hat{\boldsymbol{\imath}}(t)}{\mathrm{dt}}=\Omega\hat{\boldsymbol{\jmath}},\quad \frac{\mathrm{d}\hat{\boldsymbol{\jmath}}(t)}{\mathrm{dt}}=-\Omega\hat{\boldsymbol{\imath}}
$$
Since $\boldsymbol\Omega=\Omega\hat{\boldsymbol{k}}$ and $\hat{\boldsymbol{\imath}}=\hat{\boldsymbol{\jmath}}\times\hat{\boldsymbol{k}},~\hat{\boldsymbol{\jmath}}=\hat{\boldsymbol{k}}\times\hat{\boldsymbol{\imath}}$, they can be also written as
$$
\frac{\mathrm{d}\hat{\boldsymbol{\imath}}}{\mathrm{dt}}=\boldsymbol\Omega\times\hat{\boldsymbol{\imath}},\quad \frac{\mathrm{d}\hat{\boldsymbol{\jmath}}}{\mathrm{dt}}=\boldsymbol\Omega\times\hat{\boldsymbol{\jmath}}
$$

If $\boldsymbol{f}(t)$ is a vector with coordinate $(f_1,f_2,f_3)$ in the rotating frame, that is
$$
\boldsymbol {f}(t)=f_{1}(t){\hat {\boldsymbol {\imath }}}+f_{2}(t){\hat {\boldsymbol {\jmath }}}+f_{3}(t){\hat {\boldsymbol {k}}}
$$
then 
$$
{\displaystyle {\begin{aligned}{\frac {\mathrm {d} }{\mathrm {d} t}}{\boldsymbol {f}}&={\frac {\mathrm {d} f_{1}}{\mathrm {d} t}}{\hat {\boldsymbol {\imath }}}+{\frac {\mathrm {d} {\hat {\boldsymbol {\imath }}}}{\mathrm {d} t}}f_{1}+{\frac {\mathrm {d} f_{2}}{\mathrm {d} t}}{\hat {\boldsymbol {\jmath }}}+{\frac {\mathrm {d} {\hat {\boldsymbol {\jmath }}}}{\mathrm {d} t}}f_{2}+{\frac {\mathrm {d} f_{3}}{\mathrm {d} t}}{\hat {\boldsymbol {k}}}+{\frac {\mathrm {d} {\hat {\boldsymbol {k}}}}{\mathrm {d} t}}f_{3}\\&={\frac {\mathrm {d} f_{1}}{\mathrm {d} t}}{\hat {\boldsymbol {\imath }}}+{\frac {\mathrm {d} f_{2}}{\mathrm {d} t}}{\hat {\boldsymbol {\jmath }}}+{\frac {\mathrm {d} f_{3}}{\mathrm {d} t}}{\hat {\boldsymbol {k}}}+\left[{\boldsymbol {\Omega }}\times \left(f_{1}{\hat {\boldsymbol {\imath }}}+f_{2}{\hat {\boldsymbol {\jmath }}}+f_{3}{\hat {\boldsymbol {k}}}\right)\right]\\&=\left({\frac {\mathrm {d} {\boldsymbol {f}}}{\mathrm {d} t}}\right)_{\mathrm {r} }+{\boldsymbol {\Omega }}\times {\boldsymbol {f}}\end{aligned}}}
$$
where ${\displaystyle \left({\frac {\mathrm {d} {\boldsymbol {f}}}{\mathrm {d} t}}\right)_{\mathrm {r} }}$ denotes the rate of change of $\boldsymbol{f}$ as observed in the rotating coordinate system. This result is also known as the [transport theorem](https://en.wikipedia.org/wiki/Transport_theorem "Transport theorem") in analytical dynamics and is also sometimes referred to as the _basic kinematic equation_.

Note that when putting coordinates into the above the equation, it is important to be consistent in which frame are being used. For example:
$$
\frac{\mathrm{d}}{\mathrm{d}t}\begin{bmatrix}x\\y\\z\end{bmatrix}=\begin{bmatrix}\hat{\boldsymbol{\imath}},\hat{\boldsymbol{\jmath}},\hat{\boldsymbol{k}}\end{bmatrix}\begin{bmatrix}\dot{x'}\\\dot{y'}\\\dot{z'}\end{bmatrix}+\begin{vmatrix}\boldsymbol{i} & \boldsymbol{j} & \boldsymbol{k}\\0&0&\Omega\\x & y & z\end{vmatrix}
$$
where $\boldsymbol{i}, \boldsymbol{j}, \boldsymbol{k}$ are the unit basis vectors of the inertial frame.

