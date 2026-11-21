# Ideal Gas & Kinetic Theory Lab (PECTAA Inter Part-1 • Ch. 6)

> **Suggested GitHub Repository Name:** `ideal-gas-kinetic-theory-lab`
>
> **Live Demo:** `[Insert Your GitHub Pages Link Here]`

An interactive computational physics and statistical mechanics simulation built in pure JavaScript and HTML5 Canvas for **PECTAA Inter Part-1 (Class 11) Physics — Chapter 6 (Heat & Thermodynamics)** demonstrations. Designed to connect microscopic elastic molecular collisions with macroscopic thermodynamic laws, this simulator features a movable piston chamber, live $P\text{–}V$ indicator curves (Isothermal vs. Adiabatic), and a real-time Maxwell–Boltzmann speed distribution plot.

## Key Features

- **Spatial Hash Grid Broad-Phase Engine (`SpatialHashGrid`):** Partitions the gas chamber into uniform grid cells for $O(N)$ expected collision detection, sustaining 60 FPS with up to 420 colliding molecules.

- **Elastic Impulse & Moving Piston Physics:** Resolves momentum-conserving particle-particle and moving-wall collisions so compressing the piston imparts mechanical work ($W = P\Delta V$) directly into molecular kinetic energy.

- **Live** $P\text{–}V$ **Indicator Diagram:** Plots the gas state $(V, P)$ in real time against anchored theoretical **Isotherm (**$PV = \text{const}$**)** and steeper **Adiabatic (**$PV^\gamma = \text{const}$**)** curves.

- **Real-Time Maxwell–Boltzmann Histogram:** Bins instantaneous molecular speeds ($v$) and overlays the theoretical distribution curve alongside the live root-mean-square speed ($v_{\text{rms}}$) marker.

- **6 Built-in Thermodynamic Experiments:**
  1. **Adiabatic Piston (**$Q = 0, Q = \Delta U + W$**):** Insulated walls where piston compression heats the gas.

  2. **Boyle's Law (Isothermal,** $T = \text{const}$**):** Heat-bath coupling verifying $P_1V_1 = P_2V_2$.

  3. **Charles's Law (Isobaric,** $P = \text{const}$**):** Free-floating piston expanding proportionally with temperature ($V \propto T$).

  4. **Gay-Lussac's Law (Isochoric,** $V = \text{const}$**):** Rigid chamber demonstrating $P \propto T$.

  5. **Light & Heavy Gas Mixture (**$\text{He} + \text{Ar}$**):** Demonstrates equipartition of translational kinetic energy ($\langle E_k \rangle = \frac{3}{2}k_BT$) and $v_{\text{rms}} \propto 1/\sqrt{M}$.

  6. **Brownian Motion Tracer:** Tracks the erratic random walk of a heavy smoke/pollen grain bombarded by air molecules.

## PECTAA Inter Part-1 (Ch. 6) Physics Equations

1. **Ideal Gas Equation of State:**

   $$
   PV = nRT = Nk_BT
   $$

2. **Kinetic Pressure of an Ideal Gas:**

   $$
   P = \frac{1}{3}\rho \langle v^2 \rangle = \frac{Nm\langle v^2 \rangle}{3V}
   $$

3. **Translational Kinetic Energy & Absolute Temperature:**

   $$
   \langle E_k \rangle = \frac{1}{2}m\langle v^2 \rangle = \frac{3}{2}k_BT
   $$

4. **Root-Mean-Square (RMS) Molecular Speed:**

   $$
   v_{\text{rms}} = \sqrt{\frac{3k_BT}{m}} = \sqrt{\frac{3RT}{M}}
   $$

5. **First Law of Thermodynamics (PECTAA Notation):**

   $$
   Q = \Delta U + W \quad (W = P\Delta V)
   $$

6. **Isothermal vs. Adiabatic Processes:**

   $$
   PV = \text{const} \quad \text{vs.} \quad PV^\gamma = \text{const}
   $$

## Getting Started

No build tools, bundlers, or external dependencies are required.

1. **Clone the repository:**

   ```
   git clone https://github.com/zaindev210/ideal-gas-kinetic-theory-lab.git
   cd ideal-gas-kinetic-theory-lab

   ```

2. **Rename entry file & run locally:**
   Rename `ideal-gas.html` to `index.html` and open it directly in any modern browser.


## Tech Stack

- **Physics & Algorithms:** Vanilla JavaScript (ES6+ Spatial Hash Grid & Impulse Collision Solver)

- **Visualization:** HTML5 2D Canvas API (Chamber View, $P\text{–}V$ Indicator Plot, Maxwell–Boltzmann Histogram)

- **UI & Styling:** Tailwind CSS & JetBrains Mono scientific telemetry

## License

Open-source under the **MIT License** — ideal for classroom lectures, college science exhibitions, and computational physics portfolios.
