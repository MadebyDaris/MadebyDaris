# Daris Idirene

**Electrical Engineering Student | Computer Architecture | RISC-V Hardware Acceleration | Hardware-Software Co-Design | Novel Compute Paradigms**

<div align="left">
  <a href="https://madebydaris.github.io/"><img src="https://img.shields.io/badge/Portfolio-madebydaris.github.io-blue?style=for-the-badge&logo=github" alt="Website" /></a>
  <a href="https://www.linkedin.com/in/daris-idirene-661a66341/"><img src="https://img.shields.io/badge/LinkedIn-Daris_Idirene-0077B5?style=for-the-badge&logo=linkedin" alt="LinkedIn" /></a>
  <a href="https://www.researchgate.net/profile/Daris-Idirene"><img src="https://img.shields.io/badge/ResearchGate-Daris_Idirene-00CCBB?style=for-the-badge&logo=researchgate" alt="ResearchGate" /></a>
  <a href="https://x.com/ByDaris"><img src="https://img.shields.io/twitter/follow/ByDaris?style=for-the-badge&color=black&logo=x" alt="X" /></a>
</div>

## Technical Stack & Architectures

**Languages & Systems:**
![Julia](https://img.shields.io/badge/Julia-9558B2?style=flat-square&logo=julia&logoColor=white) ![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white) ![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white) ![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white) ![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![MATLAB](https://img.shields.io/badge/MATLAB-0076A8?style=flat-square&logo=mathworks&logoColor=white) ![](https://img.shields.io/badge/Scala-%23DC322F.svg?logo=scala&logoColor=white)

**Hardware Description & EDA Tooling:**
![SystemVerilog](https://img.shields.io/badge/SystemVerilog-0052CC?style=flat-square) ![VHDL](https://img.shields.io/badge/VHDL-0052CC?style=flat-square) ![Verilator](https://img.shields.io/badge/Verilator-FF9900?style=flat-square) ![Vivado](https://img.shields.io/badge/Xilinx_Vivado-000000?style=flat-square) ![KLayout](https://img.shields.io/badge/KLayout-2EA44F?style=flat-square) ![SPICE](https://img.shields.io/badge/SPICE/Xyce-D22128?style=flat-square) ![KiCad](https://img.shields.io/badge/KiCad-314CB6?style=flat-square&logo=kicad&logoColor=white)



I'm an Electrical Engineering student (CPGE MPSI/PSI background) transitioning to the advancing to Master's level studies in Electrical Engineering. My work sits at the boundary of hardware design and the compilers/software that target it. I ahve a keen interest for RISC-V hardware accelerators, and really interested in alternative computing paradigms like HDC, and write the tooling (schedulers, RTL emitters, EDA tools in general) needed to actually get a custom datapath from an algorithm into silicon.

I got here through device physics simulating quantum transport and memristive crossbars taught me *why* a piece of hardware behaves the way it does before I started asking how to make it faster. That's the thread running through everything below: understand the physical or mathematical structure of a problem, then design the smallest, most efficient piece of hardware that solves it.

- Designing and verifying **RISC-V coprocessors** (RoCC / CV-X-IF) for domain-specific acceleration.
- Building **Nexus-V**, a Julia-to-RTL hardware acceleration framework for RISC-V.
- Nanofabrication Engineering Intern at **Alice & Bob**, working hands-on with the cleanroom processes that put silicon designs into the physical world, and EDA tools.
- Preparing for advanced coursework in Computer Architecture and microelectronics.
## Research Interests
- **Computer Architecture & Hardware Acceleration** custom coprocessors, RoCC/CV-X-IF integration, dataflow-graph-to-RTL compilation.
- **RISC-V** open ISA extension design, accelerator dispatch, Chipyard/X-HEEP SoC integration.
- **Novel Computing Paradigms** Hyperdimensional Computing, neuromorphic/memristive architectures, and other post-CMOS/post-von-Neumann directions.
- **Electronic Design Automation** the tooling layer (schedulers, emitters, layout engines) between an algorithm and a synthesizable design.
- **Emerging Device Physics** quantum transport, memristive switching, and hardware for post-quantum cryptography.

## Flagship Projects
### [Nexus-V](https://github.com/MadebyDaris/NexusV) —A Hardware Acceleration Framework for RISC-V
`Julia` `SystemVerilog` `RISC-V` `CV-X-IF` `Verilator`

An open-source framework that turns a computation described in Julia into a library of hand-tuned IP blocks which are tuned into a pipelined, **CV-X-IF-compliant** coprocessor that plugs into the **X-HEEP** RISC-V microcontroller. The goal is to make writing a custom RISC-V accelerator look less like hand-scheduling pipeline stages from scratch and more like describing the math.
- A dataflow IR (`HWGraph`) with a **multi-cycle-aware ASAP scheduler** that correctly chains operations of different latencies (e.g., `MUL` vs `ADD`).
- A **Verilog emitter** that produces correctly pipelined SystemVerilog with automatic register insertion and a standardized `done_o` handshake.
- A **primitive library** of hand-written IP (SIMD MAC, saturating arithmetic, Barrett reduction for modular/NTT-style math) that shares the same interface as auto-generated datapaths.
- An **auto-generated dispatcher** so both compiled and hand-optimized accelerators route through one CV-X-IF shell — independently Verilator-verified.
- Actively working toward full-system simulation on X-HEEP and a PPA (power/performance/area) benchmarking harness.

### [hyperdim-rocc](https://github.com/MadebyDaris/hyperdim-rocc)  RoCC Accelerator for Hyperdimensional Computing
`Chisel/Scala` `Chipyard` `RISC-V` `RoCC`

A custom Rocket Custom Coprocessor built in the **Chipyard** framework that accelerates **Hyperdimensional Computing** an alternative, brain-inspired compute paradigm that represents and manipulates information as very-high-dimensional binary vectors instead of scalars.

- Computes Hamming distance between memory-resident hypervectors in hardware.
- A single instruction classifies a query hypervector against an entire associative memory of class vectors, streaming data directly from the L1 data cache.
- Runtime-configurable vector length via a dedicated instruction, rather than a compile-time constant.
- Verified with bare-metal RISC-V test programs on Chipyard's Verilator simulator.

The projects below are where I built the device-level and tooling intuition that now feeds into the architecture work above.

| Domain | Project | What it does |
| :--- | :--- | :--- |
| **Quantum Transport** | **[NEGF Quantum Transport Simulator](https://github.com/MadebyDaris/ResonantTunnelingDiodeSimulator)** | Non-Equilibrium Green's Function solver modeling electron tunneling in Resonant Tunneling Diodes |
| **Neuromorphic Devices** | **[Memristive Crossbar Analysis](https://github.com/MadebyDaris/memris-research)** | Simulation of HP-type memristors to analyze IR-drop and sneak-path currents in crossbar arrays |
| **Neuromorphic / FPGA** | **[Spike LIF-FPGA](https://github.com/MadebyDaris/spike-lif-fpga)** | SystemVerilog Leaky Integrate-and-Fire neuron on FPGA, benchmarked against a Julia software model |
| **Circuit Simulator Tooling** | **[Jyce.jl](https://github.com/MadebyDaris/Jyce.jl)** + **[XyceSolver](https://github.com/MadebyDaris/XyceSolver)** | Julia bindings (via CxxWrap) for Sandia's Xyce parallel circuit simulator, with Verilog-A plugin support |
| **EDA Tooling** | **[Gdstk.jl](https://github.com/MadebyDaris/Gdstk.jl)** | Julia wrapper for `gdstk`, exposing GDSII/OASIS layout geometry and boolean operations for chip layout |
| **RF Engineering** | **[2.4 GHz CMOS LNA Design](https://github.com/MadebyDaris/LNA-2-4GHz-induc-degen-casc-design)** | Inductively-degenerated cascode LNA design and noise-figure analysis |

---

## Experience

### Nanofabrication Engineering Intern (Alice & Bob)
Working hands-on in semiconductor cleanroom environments on fabrication processes, automated optical inspection, and characterization workflows for superconducting quantum computing hardware. This is the physical counterpart to the architecture work above a direct look at what it actually takes to turn a design into working silicon, and the process/yield constraints that architecture decisions eventually have to respect.

## Achievements

- **2nd Place** Hackathon 2025 with ANFR, Paris (Hybrid physics-data radio propagation model)
- **AI Coding Competition** American University of Sharjah (AUS/ASCC), UAE
- **First Slingshot Coding Competition** Participant

Please reach out :D
