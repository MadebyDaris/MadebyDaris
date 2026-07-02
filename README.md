# Daris Idirene (MadebyDaris)

**Electrical Engineering Student | Semiconductor Devices | Scientific Computing | Hardware Design**

[![Jyce.jl · MadebyDaris](https://img.shields.io/badge/Jyce.jl-MadebyDaris-blue?style=for-the-badge&logo=github&logoColor=white)](https://github.com/MadebyDaris/Jyce.jl)
[![Inertia · MadebyDaris](https://img.shields.io/badge/Inertia-MadebyDaris-blue?style=for-the-badge&logo=github&logoColor=white)](https://github.com/MadebyDaris/Inertia)
[![GitHub stars](https://img.shields.io/github/stars/MadebyDaris/Inertia?style=for-the-badge&logo=github)](https://github.com/MadebyDaris/Inertia/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/MadebyDaris/Inertia?style=for-the-badge&logo=github)](https://github.com/MadebyDaris/Inertia/network/members)
[![Last commit](https://img.shields.io/github/last-commit/MadebyDaris/Inertia?style=for-the-badge&logo=github)](https://github.com/MadebyDaris/Inertia/commits)
[![Commit activity (year)](https://img.shields.io/github/commit-activity/y/MadebyDaris/Inertia?style=for-the-badge&logo=github)](https://github.com/MadebyDaris/Inertia/graphs/commit-activity)

**Core**
![Rust](https://img.shields.io/badge/-Rust-000000?style=flat&logo=rust&logoColor=white)
![C++](https://img.shields.io/badge/-C++-00599C?style=flat&logo=c%2B%2B&logoColor=white)
![Python](https://img.shields.io/badge/-Python-3776AB?style=flat&logo=python&logoColor=white)
![Julia](https://img.shields.io/badge/-Julia-8A4AFF?style=flat&logo=julia&logoColor=white)
![CUDA](https://img.shields.io/badge/-CUDA-76B900?style=flat&logo=nvidia&logoColor=white)

**Hardware & EDA**
![SystemVerilog](https://img.shields.io/badge/-SystemVerilog-B02F2F?style=flat)
![Verilator](https://img.shields.io/badge/-Verilator-003366?style=flat)
![KiCad](https://img.shields.io/badge/-KiCad-3145A4?style=flat&logo=kicad&logoColor=white)
![LTspice](https://img.shields.io/badge/-LTspice-CA2026?style=flat&logo=analogdevices&logoColor=white)
![OpenGL](https://img.shields.io/badge/-OpenGL-5586A4?style=flat&logo=opengl&logoColor=white)

**Workflow**
![Linux](https://img.shields.io/badge/-Linux-FCC624?style=flat&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/-Git-F05032?style=flat&logo=git&logoColor=white)

**Contact**

[![Website](https://img.shields.io/badge/Portfolio-madebydaris.github.io-blue?style=for-the-badge&logo=github)](https://madebydaris.github.io/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Daris_Idirene-0077B5?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/daris-idirene-661a66341/)
[![ResearchGate](https://img.shields.io/badge/ResearchGate-Daris_Idirene-00CCBB?style=for-the-badge&logo=researchgate)](https://www.researchgate.net/profile/Daris-Idirene)
[![X](https://img.shields.io/twitter/follow/ByDaris)](https://x.com/ByDaris)

---

Electrical Engineering student with a background in theoretical physics and scientific computing. My interests lie in semiconductor devices, hardware-software co-design, and the numerical simulation of emerging computing architectures. I enjoy building high-performance engineering software that bridges device physics and hardware implementation.

## Currently

- Nanofabrication Engineering Intern at **Alice & Bob**
- Building scientific simulation software in **Rust** and **Julia**
- Preparing to pursue graduate studies in a top tier insitution in Electrical Engineering

---

## Experience

### Nanofabrication Engineering Intern — Alice & Bob
Working in semiconductor cleanroom environments on fabrication processes, optical inspection, and characterization workflows for quantum computing hardware.

- Cleanroom fabrication
- Optical inspection
- Semiconductor process characterization

---

## Background

I study at **Université Paris-Saclay**, with training in the **CPGE (MPSI/PSI)** curriculum, where I built a rigorous foundation in mathematical modelling and system design.

I've been programming for over a decade, gradually transitioning from general software engineering toward scientific computing and hardware-oriented engineering. My academic focus has shifted toward the physical limits of computing I try to bring engineering problems back to their underlying linear algebra and analysis.

My current projects focus on quantum transport, neuromorphic architectures, and RF engineering, through simulation engines and physics-aware hardware design as well as building EDA tools to get a better idea on how they work.

---

## Projects

| Domain | Project | Tech Stack |
| :--- | :--- | :--- |
| **Quantum Physics** | **[NEGF Quantum Transport Simulator](https://github.com/MadebyDaris/ResonantTunnelingDiodeSimulator)**<br>Solver using the Non-Equilibrium Green's Function formalism to model electron transport and tunneling in Resonant Tunneling Diodes (RTDs). | `Julia` `Numerical Methods` |
| **Neuromorphic** | **[Memristive Crossbar Analysis](https://github.com/MadebyDaris/memris-research)**<br>Simulation of HP-type memristors to analyze IR-drop and sneak path currents in neuromorphic computing architectures. | `SPICE` `Julia` `Python` |
| **Circuit Simulation Tooling** | **[Jyce.jl](https://github.com/MadebyDaris/Jyce.jl)** + **[XyceSolver](https://github.com/MadebyDaris/XyceSolver)**<br>Julia bindings (via CxxWrap) for Sandia's Xyce parallel circuit simulator, including a C++ wrapper layer and Verilog-A plugin support. Used to run memristor examples with the VTEAM model. | `Julia` `C++` `CxxWrap` `Verilog-A` |
| **Neuromorphic / Hardware** | **[Spike LIF-FPGA](https://github.com/MadebyDaris/spike-lif-fpga)**<br>SystemVerilog implementation of a Leaky Integrate-and-Fire neuron on FPGA, benchmarked against a Julia software model. | `SystemVerilog` `Verilator` `Julia` |
| **Simulation** | **[Inertia Physics Engine](https://github.com/MadebyDaris/Inertia)**<br>GLSL compute-shader engine for parallel N-body dynamics and Schrödinger equation visualization. | `Rust` `OpenGL` `GLSL` |
| **RF Engineering** | **[2.4 GHz CMOS LNA Design](https://github.com/MadebyDaris/LNA-2-4GHz-induc-degen-casc-design)**<br>Design and noise figure analysis of an inductively degenerated cascode Low Noise Amplifier for RF applications. | `CMOS` `Impedance Matching` |
| **EDA Tooling** | **[Gdstk.jl](https://github.com/MadebyDaris/Gdstk.jl)**<br>Julia wrapper for `gdstk`, a GDSII/OASIS layout engine, exposing geometry, boolean operations, and path tools for chip layout work. | `Julia` `CxxWrap` `GDSII` |

---


## Engineering Interests

- Semiconductor Devices
- Electronic Design Automation
- Scientific Computing
- High Performance Computing
- RF IC Design
- Neuromorphic Computing
- Numerical Methods
- Hardware/Software Co-design
- Circuit Simulator Tooling (Xyce)

---

## Achievements

- **2nd Place** — Hackathon 2025 with ANFR, Paris
- **AI Coding Competition** — American University of Sharjah (AUS/ASCC), UAE
- **First Slingshot Coding Competition** — Participant

---

I enjoy contributing to open-source scientific software and exploring how computation can accelerate advances in semiconductor technologies and emerging computing architectures.
