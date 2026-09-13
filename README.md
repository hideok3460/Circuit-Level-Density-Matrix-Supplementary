# Circuit-Level Density-Matrix Supplementary Material

This repository is prepared as the companion archive for the manuscript **“Circuit-Level Density-Matrix Channel-Equivalence Verification of a Five-Qubit Coherent EPR-State Transfer Network with a Two-Component GHZ Resource Family.”**

It contains two supplementary components. **Supplementary Material S1** (`Supplementary_Appendix_B.pdf/.tex`) gives the self-contained Dirac-expanded controlled-X derivation moved from the main manuscript. **Supplementary File S2** (`verification_canonical_noncanonical_CP_TNI.ipynb`) is the executed same-backend IBM Quantum workflow for the canonical `(M1,M2)=(0,0)` and noncanonical `(0,1)` resources.

The S2 notebook records the combined `ibm_phoenix` job `daj7e68mhr3c73e8kotg`, containing 216 circuits with 4096 shots per circuit. It performs receiver-state tomography, reconstructs four-probe unnormalized code-space blocks, fits a completely-positive trace-non-increasing (CP-TNI) Choi matrix by convex least squares, and evaluates 500-sample multinomial bootstrap intervals for process-level metrics. No error mitigation or SPAM separation is applied. The bootstrap intervals quantify finite-shot uncertainty for this submitted batch and do not measure run-to-run drift.

The CSV files reproduce the central same-backend state and CP-TNI process summaries used in the manuscript. The PNG files are the publication outputs showing the CP-TNI Pauli-transfer matrices, bootstrap process metrics, and physicality diagnostics.
