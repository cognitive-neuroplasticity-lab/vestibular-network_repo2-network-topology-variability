# Vestibular Network Topology Variability

A neuroimaging analysis project examining inter-individual differences in functional network topology within brain systems relevant to vestibular and spatial cognition.

This repository extends the vestibular track from dataset readiness into computational analysis using open resting-state fMRI data, graph theory, and reproducible workflows.

---

## Project Aim

To test whether candidate vestibular-related brain networks show meaningful variability in topological organization across individuals, and to build a scalable framework for future vestibular-specific and behaviour-linked analyses.

---

## Why This Repository Uses an Accessible Normative Sample

The long-term scientific target of this research track is vestibular-network organization using large open datasets such as ID1000 / AOMIC. However, direct full-cohort ingestion can be unnecessarily heavy during early portfolio-stage development.

For this repository, an openly accessible resting-state sample was used to prioritize:

* rapid pipeline construction
* transparent reproducibility
* graph-theoretic implementation
* proof-of-concept variability analysis

This is a deliberate methodological staging decision rather than a substitute for future larger-cohort work.

---

## Scientific Background

Vestibular cognition extends beyond balance and reflexes. It contributes to:

* self-location
* multisensory integration
* spatial transformation
* navigation
* body representation
* environmental orientation

These functions are supported by distributed networks involving regions such as:

* temporo-parietal junction
* posterior insula
* inferior parietal lobule
* precuneus
* hippocampal formation
* parahippocampal cortex
* cerebellar vestibular zones

A network-science approach is therefore appropriate.

---

## Dataset Base

* Open resting-state fMRI sample
* Healthy participants
* Proof-of-concept subset: 5 subjects
* Whole-brain atlas workflow

---

## Methods

The repository implemented the following pipeline:

1. Load open resting-state functional MRI data
2. Extract ROI time series using a standard cortical atlas
3. Estimate subject-level functional connectivity matrices
4. Threshold matrices into graphs
5. Compute topology metrics:

   * density
   * clustering coefficient
   * connected components
6. Compare variability across participants
7. Visualize ranking, spread, and future scaling paths

---

## Main Findings

* Functional connectivity graphs were successfully generated across subjects
* Network topology metrics differed across individuals
* Higher graph density aligned with higher clustering
* Most subjects showed fully connected graphs, while some showed fragmented organization
* Inter-individual differences were observable even in a small pilot sample

---

## Repository Workflow

### Notebook 1 - Data Access and Sample Selection

Established a feasible open-data workflow and defined vestibular candidate regions.

### Notebook 2 - Connectivity and Graph Construction

Built subject-level connectivity matrices and derived graph metrics.

### Notebook 3 - Topology Variability Analysis

Quantified between-subject differences in density, clustering, and integration.

### Notebook 4 - Visual Overview

Generated non-redundant interpretation figures and future scaling roadmap visuals.

### Notebook 5 - Summary and Next Steps

Consolidated findings, limitations, and forward research directions.

---

## Why Whole-Brain Atlases Were Used Initially

Early-stage vestibular neuroimaging faces a common challenge: the vestibular cortex is distributed and not captured by one universally accepted atlas.

A whole-brain atlas was used here to:

* ensure reproducibility
* avoid arbitrary ROI selection
* enable immediate graph analysis
* create a baseline pipeline for later vestibular-focused refinement

Future repositories will narrow analyses to literature-derived vestibular candidate ROIs.

---

## Limitations

* Pilot sample size
* Accessible sample rather than full target cohort
* Whole-brain approximation rather than vestibular-only network graph
* No behavioural spatial-cognition linkage yet
* Threshold choices may influence graph metrics

---

## Future Directions

* Expand to larger normative cohorts
* Use vestibular candidate ROI graphs only
* Link topology to mental rotation and spatial cognition measures
* Build predictive models of spatial performance
* Evaluate robustness across preprocessing and threshold settings

---

## Tools Used

* Python
* Pandas
* NumPy
* Nilearn
* NetworkX
* Matplotlib
* Seaborn
* Google Colab

---

## Maintained By

Aditya Sundaray
