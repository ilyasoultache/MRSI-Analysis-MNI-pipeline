# MRSI Analysis Pipeline (MNI)

Official Magnetic Resonance Spectroscopic Imaging (MRSI) analysis pipeline from the **Brain Tumor Research Group** at the **Montreal Neurological Institute (MNI)**.

## Mission
We aim to **democratize access to multi-voxel MRSI** and support **more standardized clinical integration**.

## Overview
This repository provides an end-to-end workflow for multi-voxel MRSI processing and metabolite quantification, designed to be reproducible and clinically oriented.

**Core steps (high level):**
1. MRI preprocessing (denoise, brain extraction)
2. MRSI conversion + preprocessing (frequency/phase, ECC, water removal)
3. Coregistration to anatomical MRI
4. Basis-set generation (sequence-matched)
5. Partial-volume estimation/correction (GM/WM/CSF)
6. Spectral fitting + QC filtering
7. Outputs: voxel-wise metabolite maps + ROI summaries (as configured)

## What this repository contains
- Documentation and usage instructions for the MRSI analysis pipeline
- Recommended workflows for processing, fitting, and QC

This work builds on open-source tools commonly used in MRSI workflows:
- **HD-BET** (brain extraction)
- **ANTs** (MRI preprocessing/denoising)
- **FSL-MRS** (MRS preprocessing + fitting)
- **FID-A** (basis set generation)
