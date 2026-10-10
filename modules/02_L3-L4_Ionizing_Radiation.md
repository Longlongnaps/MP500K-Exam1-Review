# Module 02 — L3–L4: Ionizing Radiation and Radiation Fields

[← Home](../README.md) · [← Module 01](01_L1-L2_Foundations.md) · [Next: Module 03 →](03_L5-L6_Atomic_Structure.md)

**Source:** `Lecture_3.pdf` (original L3 & L4 joint lecture, pp. 1–24), `Lecture_4.pdf` (continuation, pp. 1–16).  
**Exam guide:** radiation classification, precision, four fluence quantities = **Basic**; differential/alternative/planar fluence = **Advanced**.

## 1. Introduction

**Ionizing radiation** has sufficient energy to detach electrons from atoms/molecules. **Excitation** raises a bound electron to another bound state; **ionization** removes it from the atom.

- **Radiological physics:** ionizing radiation, its interactions with matter, and the energy transferred/absorbed.
- **Radiation dosimetry:** quantitative assessment of radiation energy deposition.
- Lecture examples include medicine, nuclear reactors, screening, industrial radiography, sterilization and chemical modification.

## 2. Types and sources

| Type | Key physical origin/description |
|:--|:--|
| X-ray | Atomic transitions (characteristic), or acceleration/deceleration (bremsstrahlung) |
| Gamma ray | Nuclear transitions; annihilation photons may also be described as gamma rays |
| Fast electron | Photoelectron, Compton electron, beta, delta ray, Auger, IC, etc. |
| Heavy charged particle | Proton, deuteron, triton, alpha, heavier ions |
| Neutron | Nuclear sources/reactions; uncharged, indirectly ionizing |

**X-ray vs gamma ray:** principal distinction is **origin**, not photon energy; both obey $E=h\nu=hc/\lambda$.

For slow neutrons the nonrelativistic relation is $K=\tfrac12mv^2$. Thermal-neutron benchmark (lecture): **$K\approx0.025\ \mathrm{eV}$**, **$v\approx2200\ \mathrm{m/s}$**. Heavier charged particles require relativistic kinematics at sufficiently high energy.

**Direct ionization:** fast charged particle → repeated Coulomb interactions → ionization/excitation.  
**Indirect ionization:** photon/neutron → energetic secondary charged particle → ionization/excitation.

## 3. Random nature of radiation fields

### Stochastic vs non-stochastic

Single detected **counts** are stochastic (vary between repeated measurements). Expected fluence/rate are defined as **non-stochastic** quantities under fixed conditions.

For Poisson counting with mean $\Lambda$:

$$
P(N=k)=\frac{\Lambda^k e^{-\Lambda}}{k!},\quad
\mathbb E[N]=\mathrm{Var}(N)=\Lambda,\quad
\sigma_N=\sqrt{\Lambda}\approx\sqrt N.
$$

For large $\Lambda$, Poisson counts can be approximately normal. The normal distribution does **not** generally satisfy variance = mean; that equality comes from the underlying Poisson model.

With $n$ independent repeated equal-duration measurements:

$$
\mathrm{SEM}=\frac{\sigma_N}{\sqrt n},\qquad
\frac{\sigma_N}{\Lambda}=\frac1{\sqrt\Lambda},\qquad
\frac{\mathrm{SEM}}{\Lambda}=\frac1{\sqrt{n\Lambda}}.
$$

If measuring $N$ counts during a known time $t$:

$$
R=\frac Nt,\qquad \sigma_R\approx\frac{\sqrt N}{t}.
$$

**Interpretation:** More counts reduce **relative** counting uncertainty, although the absolute standard deviation $\sqrt N$ increases.

Sample standard deviation from repetitions:

$$
s=\sqrt{\frac1{n-1}\sum_{i=1}^n(N_i-\overline N)^2}.
$$

## 4. Description of the radiation field

| Quantity | Symbol and definition | Units |
|:--|:--|:--|
| Fluence | $\Phi=dN_e/da$ | $\mathrm{m^{-2}}$ or $\mathrm{cm^{-2}}$ |
| Fluence rate | $\varphi=d\Phi/dt$ | $\mathrm{m^{-2}\,s^{-1}}$ |
| Energy fluence | $\Psi=dR/da$ | $\mathrm{J\,m^{-2}}$ |
| Energy fluence rate | $\psi=d\Psi/dt$ | $\mathrm{J\,m^{-2}\,s^{-1}}$ |

$N_e$ is **expected particle count**, $R$ is expected radiation energy, and $da$ is the **great-circle area of an infinitesimal sphere**. Do not silently substitute the area of a fixed plane.

For **monoenergetic** radiation of energy $E$:

$$
\Psi=E\Phi,\qquad\psi=E\varphi.
$$

**Fluence rate ≠ count rate:** fluence rate has a per-area factor; the detector count rate may also depend on efficiency and response.

## 5. Differential distribution vs energy and angle

A differential fluence rate can depend on energy $E$ and direction $(\theta,\beta)$:

$$
\varphi'(\theta,\beta,E)=\frac{d\varphi}{d\Omega\,dE},\qquad
d\Omega=\sin\theta\,d\theta\,d\beta.
$$

Total over angles and energies:

$$
\varphi=\int_0^\pi\int_0^{2\pi}\int_0^{E_{\max}}
\varphi'(\theta,\beta,E)\sin\theta\,dE\,d\beta\,d\theta.
$$

Energy-only spectrum after angle integration:

$$
\varphi=\int\varphi'(E)\,dE,\qquad
\psi'(E)=E\varphi'(E),\qquad
\psi=\int E\varphi'(E)\,dE.
$$

**Figure interpretation (L4 pp. 6–7):** area under particle-fluence spectrum = total **particle fluence rate**. Area under energy-weighted spectrum = total **energy fluence rate**. Even if $\varphi'(E)$ is flat, $\psi'(E)$ increases linearly with $E$.

## 6. Alternative definitions and planar fluence

**Chilton's theorem / track-length formulation:**

$$
\Phi=\lim_{\Delta V\to0}\frac{\mathbb E[\sum_i\Delta \ell_i]}{\Delta V}.
$$

The sum of tracks has units of length; divided by volume gives inverse area, consistent with fluence.

**Planar fluence:** crossings of a *fixed plane* are counted from either side with **scalar** addition. For a beam making angle $\theta$ with the surface normal:

$$
\Phi_p=\Phi\,|\cos\theta|.
$$

For an isotropic field:

$$
\frac{\varphi_p}{\varphi}=
\frac{\int_0^\pi|\cos\theta|\sin\theta\,d\theta}{\int_0^\pi\sin\theta\,d\theta}=\frac12.
$$

**Net flow** instead uses the signed $\cos\theta$ and is **zero** for an isotropic field. The absolute value matters: the lecture describes crossings **in either direction**.

### Can you explain without notes?

- Standard deviation vs standard error of the mean?
- Difference between $\Phi$, $\varphi$, $\Psi$ and $\psi$?
- Why does an isotropic field have planar fluence rate $\varphi/2$, but zero net flow?
