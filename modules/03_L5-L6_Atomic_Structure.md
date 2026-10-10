# Module 03 — L5–L6: Atomic Structure

[← Home](../README.md) · [← Module 02](02_L3-L4_Ionizing_Radiation.md) · [Next: Module 04 →](04_L7-L9_Xray_Attenuation.md)

**Source:** `Lecture_5.pdf` pp. 3–32; `Lecture_6.pdf` pp. 2–22.  
**Exam guide:** atomic models, hydrogen energy diagram, quantum numbers and electron configuration = **Basic**; Bohr electron and spectral series = **Solid**; multi-electron atoms = **Advanced**.

## L5 · 1. Basic models of the atom

| Model | Core proposal | Limitation |
|:--|:--|:--|
| Dalton | Elements consist of atoms; simple whole-number ratios in compounds | Atoms actually have substructure |
| Thomson (1897) | Electrons embedded in positively charged sphere; **no nucleus** | Cannot explain large-angle alpha scattering |
| Rutherford (1911) | Tiny dense positive nucleus, most of atom empty | Accelerating classical orbit electron should radiate/collapse |
| Bohr (1913) | Allowed quantized nonradiating electron orbits and transitions | Simplified hydrogen-like model |

**Bohr's four postulates (lecture pp. 7–8):**

1. Coulomb attraction provides centripetal force, $m_ev^2/r=Ze^2/(4\pi\varepsilon_0r^2)$.
2. Electron does **not** radiate in an allowed stationary orbit.
3. Allowed orbital angular momentum is quantized: $L=n\hbar$, with $n=1,2,\dots$.
4. An electron transition exchanges a photon of energy $\lvert E_i-E_f\rvert=h\nu=hc/\lambda$.

## L5 · 2. Properties of Bohr electron

For **one-electron atoms/ions** with a heavy-nucleus, nonrelativistic approximation:

$$
\boxed{r_n=a_0\frac{n^2}{Z}},\qquad a_0=5.29\times10^{-11}\ \mathrm m=0.529\ \text{Å}
$$

$$
\boxed{v_n=\alpha c\frac Z n},\qquad\alpha\simeq1/137
$$

$$
\boxed{E_n=-13.6\frac{Z^2}{n^2}\ \mathrm{eV}}
$$

For ground-state hydrogen ($n=Z=1$): $r_1=0.529\ \text{Å}$, $v_1\approx2.19\times10^6\ \mathrm{m/s}$, $E_1=-13.6\ \mathrm{eV}$.

**Meaning of negative energy:** the zero is defined at an electron/nucleus infinite separation (ionization limit). A bound electron is below that energy. The formula is **not** universally valid for every electron of a multi-electron atom.

## L5 · 3. Energy levels and transitions

**Hydrogen energy diagram (lecture pp. 16–18):**

| $n$ | $E_n$ (eV) |
|:--:|--:|
| 1 | −13.60 |
| 2 | −3.40 |
| 3 | −1.51 |
| 4 | −0.85 |
| $\infty$ | 0.00 |

- **Excitation:** bound state $i\to f$ with $E_f>E_i$; $E_{exc}=E_f-E_i$.
- **Ionization:** bound electron removed to continuum threshold $E_\infty=0$; $E_{ion}=0-E_i$.
- **Emission:** upper $n_i$ to lower $n_f$, photon energy $E_\gamma=E_i-E_f>0$.
- **Absorption:** supplies the positive energy needed to move to a higher electronic state.

**Balmer empirical formula**, with $n_i\ge3$ and final $n_f=2$:

$$
\lambda=3646\frac{n_i^2}{n_i^2-4}\ \text{Å}.
$$

**Rydberg formula** for hydrogen:

$$
\frac1\lambda=R_\infty\left(\frac1{n_f^2}-\frac1{n_i^2}\right),\qquad
R_\infty=1.097373\times10^7\ \mathrm{m^{-1}}.
$$

| Series | $n_f$ | Region |
|:--|--:|:--|
| Lyman | 1 | Ultraviolet |
| Balmer | 2 | Visible (major lines) / limit near UV |
| Paschen | 3 | Infrared |
| Brackett | 4 | Infrared |

**Series identity is fixed by $n_f$, not $n_i$.** For any fixed $n_f$, longest wavelength comes from $n_i=n_f+1$ (smallest transition energy), shortest from $n_i\to\infty$ (series limit).

## L5 · 4. Correction for finite nuclear mass

The nucleus is not infinitely heavy: electron and nucleus orbit their mutual center of mass. Use **reduced mass**:

$$
\mu_r=\frac{m_eM}{m_e+M},\qquad R_H=\frac{\mu_r}{m_e}R_\infty.
$$

Lecture values: $R_H\approx1.09678\times10^7\ \mathrm{m^{-1}}$. Special systems: **positronium** ($e^+e^-$) and **muonic atoms** (nucleus + negative muon). Differences in reduced mass alter level energies.

## L5 · 5. Multi-electron atoms (Advanced)

The electron experiences nuclear attraction **and** electron–electron repulsion. A simple Hartree-inspired effective-charge picture uses:

$$
V(r)\approx-\frac{Z_{eff}e^2}{4\pi\varepsilon_0r}.
$$

This illustrates **shielding**. The slide's simple $Z_{eff}$ recipes are not general exact rules: energy in many-electron atoms depends on both $n$ and $l$ and on interactions, spin–orbit effects, etc.

## L6 · 6. Electron quantum numbers

| Name | Symbol | Allowed values | Meaning |
|:--|:--:|:--|:--|
| Principal | $n$ | $1,2,3,\ldots$ | Shell (K, L, M, N, …) |
| Orbital | $l$ | $0,1,\ldots,n-1$ | Subshell (s,p,d,f,g,…) |
| Magnetic | $m_l$ | $-l,\ldots,l$ | Orbital angular momentum projection |
| Spin | $m_s$ | $\pm1/2$ | Electron spin projection |

**Angular momenta:**

$$
L=\sqrt{l(l+1)}\hbar,\qquad L_z=m_l\hbar.
$$

Be careful: **Bohr's** $L=n\hbar$ and **quantum mechanical** $L=\sqrt{l(l+1)}\hbar$ come from different models.

| $l$ | Subshell | Number of orbitals $2l+1$ | Max electrons $2(2l+1)$ |
|--:|:--:|--:|--:|
| 0 | s | 1 | 2 |
| 1 | p | 3 | 6 |
| 2 | d | 5 | 10 |
| 3 | f | 7 | 14 |

A full principal shell has:

$$
N_{orbitals}=n^2,\qquad N_{electron\ states}=2n^2.
$$

**Pauli exclusion principle (lecture p. 11):** no two electrons in one atom may share the same set $(n,l,m_l,m_s)$. Therefore each spatial orbital admits at most **two electrons of opposite spin**.

## L6 · 7. Atomic electron configuration

**Aufbau principle:** occupy generally lower-energy orbitals first. A standard order is:

```text
1s → 2s → 2p → 3s → 3p → 4s → 3d → 4p → 5s → 4d → 5p
   → 6s → 4f → 5d → 6p → ...
```

**Hund's rule:** among *degenerate* orbitals of the same subshell, occupy them singly with parallel spins before pairing.

**Pauli principle:** at most 2 electrons per orbital; spins opposed when paired.

Examples from the lecture:

| Neutral atom | Ground-state configuration |
|:--|:--|
| H | $1s^1$ |
| B | $1s^22s^22p^1$ |
| N | $1s^22s^22p^3$ |
| F | $1s^22s^22p^5$ |
| Na | $1s^22s^22p^63s^1$ |

For neutral atoms, total electrons = $Z$. Some configurations deviate from a naïve filling sequence because orbitals are close in energy; the order is a teaching guide rather than an exceptionless law.

### Quick conceptual checks

- Why is **3f** forbidden but **4f** allowed? ($l\le n-1$)
- For a 2p subshell, how many *orbitals* vs *electron states*?
- Why is a **2p³** ground-state occupancy `↑ ↑ ↑` rather than `↑↓ ↑ _`?
