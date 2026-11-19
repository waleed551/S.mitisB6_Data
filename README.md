# Streptococcus mitis B6 Supporting Data

Supporting computational records for the study “Drug Targets Identified Through Subtractive Genome Analysis of Streptococcus mitis B6 with Molecular Dynamics Assessment of Homoserine Dehydrogenase.”

This repository provides the compound-screening library, original HSD model, and records from a repeated Phyre2 analysis to support inspection and reproducibility of the reported analyses.

## Repository contents

| File | Description |
|---|---|
| `HSD_original_model_3MTJ_chainA.pdb.pdb` | Recovered original HSD model, previously named `final.casp (1).pdb`. Its header records the source filename `c3mtjA_.1.pdb.sc`, indicating template 3MTJ chain A. |
| `c3mtjA_.2.alig.html` | HTML alignment for the 3MTJ chain A hit from the repeated Phyre2 analysis. |
| `c3mtjA_.2.alig.txt` | Text alignment containing sequence identity, alignment confidence, aligned positions, and gaps. |
| `c3mtjA_.2.fasta` | Pairwise target–template sequence alignment in FASTA format. |
| `c3mtjA_.2.pdb` | Model downloaded for the 3MTJ chain A hit in the repeated Phyre2 analysis. |
| `c3mtjA_.2.png` | Structural image associated with the 3MTJ chain A hit. |
| `hit_report.pdf` | Phyre2 template-search report from the repeated analysis. |
| `zinc 12000.mdb` | MOE database containing the compound library used for screening. |

## HSD modeling records

The recovered original HSD model contains 426 residues numbered 2–427. Its header identifies a source filename corresponding to PDB 3MTJ chain A.

A repeated Phyre2.2 analysis used the 426-residue sequence extracted from the original coordinates. In this run, 3MTJ chain A was the second-ranked hit, with 38% sequence identity and 100.0% reported confidence.

The alignment spans query positions 1–426. Of these, 411 residues are paired with template residues, corresponding to 96.48% of the submitted sequence. Fifteen query residues occur opposite template gaps.

These alignment metrics describe the repeated analysis. The original coordinates and the models generated during the repeated analysis should be identified separately when reporting results.

## Residue numbering

The sequence submitted for the repeated analysis starts at position 1, corresponding to residue 2 in the original model.

For example, original-model Tyr334 corresponds to query position 333. Check residue identities and numbering when comparing alignments, structures, docking contacts, and validation results.

## Using the files

- Open PDB files in a molecular structure viewer.
- Inspect the HTML, text, or FASTA alignments to examine target–template correspondence.
- Consult `hit_report.pdf` for template rankings and reported modeling metrics.
- Open `zinc 12000.mdb` using compatible MOE software to inspect the compound records.

## Interpretation and limitations

The proteins and compounds investigated in this study are computationally prioritized candidates. Experimental confirmation of HSD inhibition, antimicrobial activity, selectivity, and safety is required.

The repeated alignment identifies local uncertainty around original-model residues Glu333–Arg336. Predicted ligand contacts involving this region require cautious interpretation.

The presence of a ZINC identifier in the screening library confirms library membership. Correspondence among an identifier, chemical structure, physicochemical properties, docking score, and saved pose requires verification against the relevant molecular records.

Protein backbone RMSD and per-residue RMSF describe protein conformational behavior. Persistent ligand binding requires analysis of ligand positioning and protein–ligand contacts during the trajectories.

The files listed above provide supporting records. Reproducing the complete docking and MD workflow also requires the corresponding preparation settings, docking outputs, simulation inputs, trajectories, and analysis scripts.

## Citation

Please cite the associated manuscript when using these data. Publication details will be added when available.
