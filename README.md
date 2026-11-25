# UAV Case Study: RBDDL Model and Synthesized OS Telemetry Datasets

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

This repository contains the system model and synthesized operational datasets used to validate the Reliability-Based Monitoring (RBM) framework presented in:

> **A Stress-Driven Framework for Real-Time Software Reliability Monitoring in Complex Computing Environments**  
> Gloria Gori, Marco Papini, Alessandro Fantechi
> *Innovations in Systems and Software Engineering (ISSE)*, Springer (submitted).

## Contents

The artifacts support the 24-hour dual-level Unmanned Aerial Vehicle (UAV) case study, comprising a  bare-metal flight controller (**NXP i&#46;MX RT**) and a Linux companion computer (**NVIDIA Jetson TX2**):

* `models/` — RBDDL specification of the dual-level UAV architecture, combining MIL-HDBK-217F hardware models with NHPP-based Software Reliability Growth Models.
* `datasets/` — Synthesized 24-hour OS-level telemetry traces sampled at $\gamma = 10\text{ s}$. These datasets were used by the authors to compute the software aging stress profiles $\eta(t)$ and evaluate runtime reliability updates.

## Related Software

The reliability evaluation relies on the open-source **librbd** library and **rbdEngine** application, available separately under the AGPL license:
* [librbd Repository](https://github.com/marcopapini/librbd)
* [rbdEngine Repository](https://github.com/marcopapini/rbdEngine)

## License

The datasets and RBDDL model in this repository are licensed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

## Citation

If you use these datasets or the RBDDL model in your research, please cite the accompanying paper (see `CITATION.cff` or use the "Cite this repository" button on GitHub).
