# Virtual Research Environment for Molecular Dynamics Simulation Experiments

The thesis will design and implement a prototype of MDDash, a wizard-style web application built on JupyterHub in Kubernetes that emphasizes efficient use of HPC resources and reproducible execution captured as provenance in Jupyter notebooks; the system will support automated performance tuning of GROMACS runs (MPI/OMP and CPU/GPU configuration), integrate an analysis/visualization stage, and enable direct publication of results to an InvenioRDM repository with rich automatically extracted metadata using Gromacs Metadump, while keeping the architecture extensible for user-contributed workflows and future support of additional MD engines.

- Analyze requirements and existing MD web portals; define functional/non-functional requirements for MDDash
- Design the system architecture on JupyterHub + Kubernetes (auth via OAuth2, user isolation, workflow execution model)
- Implement the 5-stage wizard flow: preparation > tuning > production > analysis > publishing
- Implement automated tuning experiments for short benchmark runs and selection of the best resource/performance trade-off
- Integrate metadata extraction via Gromacs Metadump and create draft InvenioRDM records from results
- Deliver deployment artifacts (Helm charts), documentation, and an evaluation on representative MD use cases
