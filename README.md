# Energy-Aware Replenishment and Hierarchical Formation Control for Persistent Multi-UAV Urban Target Tracking

[![Watch Online (Interactive Video Player)](https://img.shields.io/badge/%E2%96%B6_Watch_All_Videos_Online-Interactive_Side--by--Side_Player-1d4ed8?style=for-the-badge)](https://htmlpreview.github.io/?https://github.com/ESDerg/RAS-UAVs-Battery/blob/main/index.html)

---

## Overview

This repository provides supplementary 3D trajectory comparison animations for the paper **"Energy-aware replenishment and hierarchical formation control for persistent multi-UAV urban target tracking"**.

To sustain continuous multi-UAV coverage of a moving ground target across repeated battery-replenishment cycles in urban environments, our hierarchical framework decouples flight control from energy management:
- **3D Formation NMPC:** Maintains cooperative target-tracking geometry and local 3D obstacle avoidance across staggered cruise altitudes ($z_{\mathrm{cr}} \in \{20, 30, 40\}\,\mathrm{m}$ AGL).
- **Coupled Thevenin–3D Replenishment Decision Layer (`Thevenin+3D`, Ours):** Evaluates second-order equivalent-circuit battery dynamics, nonlinear aerodynamic power demand along 3D return trajectories, and single-pad queuing delays to trigger timely autonomous battery swaps.

All closed-loop missions are conducted in **CARLA-Air** (Town10 urban environment) with $N_u = 3$ quadrotor UAVs over a nominal $T = 600\,\mathrm{s}$ horizon at a $4.0\,C$ discharge rate with a shared safety reserve of $T_{\mathrm{res}} = 60\,\mathrm{s}$, comparing our proposed **`Thevenin+3D` (`*_ours.mp4`)** against the conventional linear charge-accounting baseline **`linear+hor` (`*_base.mp4`)**.
