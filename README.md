# MechanicsFit Automate — Abaqus

Turn batches of Abaqus simulations into engineering-ready results and reports.

**Private Beta — V0.1.1** · Local Abaqus batch post-processing for repetitive engineering workflows.

MechanicsFit Automate helps you inspect and process multiple ODB files, compare cases, and prepare reviewable outputs. **ODB files stay on your machine.** There is no automatic ODB upload, engineering-result upload, or telemetry.

## What it does

- Inspect ODB contents and run batch extraction for S/Mises, U, RF, and PEEQ.
- Sum support reactions over node sets, apply user-defined engineering checks, and compare cases.
- Identify failed checks and critical cases where the selected result semantics support that comparison.
- Save and reuse workflows; export Excel tables and HTML engineering reports.

## Typical workflow

Multiple Abaqus ODBs → Inspect → Extract → Apply engineering checks → Review failed and critical cases → Compare → Export report.

The included **synthetic demonstration** contains 48 precomputed cases, four extraction tasks, three engineering checks, and a deliberately failed result. It highlights `Job_023` as a critical stress case. Demo data are illustrative and are not real Abaqus results or evidence of measured time savings.

## Download Private Beta

**Release asset: `MechanicsFit-Automate-Abaqus-V0.1.1-Private-Beta-Protected.zip`**

The download link will be added here when the protected beta package has been validated and released.

## Requirements and first run

- Windows and Python 3.11.
- A local Abaqus installation with the ODB API is required to process real ODB files. The compiled worker in this package was built and tested for Abaqus 2025's Python 3.10; other Abaqus versions are not yet supported by this protected build.
- Demo Mode works without Abaqus.

Once the ZIP is available, extract it, double-click **Start MechanicsFit.bat**, and open **Try Demo**. For real projects, configure the local Abaqus installation, select ODB files, set extraction tasks and engineering checks, then verify at least one result in Abaqus/CAE. Use **Stop MechanicsFit.bat** when finished. The app opens on an available localhost port beginning at 8503.

## Feedback and privacy

Please test on a real ODB workflow and [send beta feedback](https://docs.google.com/forms/d/e/1FAIpQLSdjNlWNsMiu5kYkezCK69NyvKMxkHKm-ay1OyB6zCO-4hKynw/viewform). Feedback is submitted only when you choose to open and complete the external form. Diagnostic bundles are generated locally and are never uploaded automatically. Please do not include confidential model data in feedback.

> **Private Beta:** MechanicsFit Automate is currently in beta. Please independently verify critical engineering results against Abaqus/CAE. It does not certify FEA correctness.

See [Beta notice](BETA_NOTICE.md) for the current scope.
