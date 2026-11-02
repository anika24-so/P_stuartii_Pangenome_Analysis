# Comparative Pangenome Analysis of *Providencia stuartii*

## Overview

This repository contains the computational outputs of comparative pangenome analysis of *Providencia stuartii*, including the environmental isolate *P. stuartii* BCSIR.

The study investigated the genomic diversity and distribution of conserved, accessory, and strain-specific genes across 31 representative *P. stuartii* genomes.

## Genome Dataset

A total of 31 *Providencia stuartii* genomes were included:

- One environmental isolate: *P. stuartii* BCSIR.
- Thirty reference genomes retrieved from the Bacterial and Viral Bioinformatics Resource Center (BV-BRC).

Reference genomes were selected based on genome quality and the availability of relevant metadata, including geographical information, isolation source, and collection year.

## Computational Workflow

### 1. Genome Annotation

All genome sequences were annotated using Prokka (v1.14.6).

The resulting GFF3 annotation files were subsequently used as input for comparative pangenome analysis.

### 2. Pangenome Analysis

Pangenome analysis was performed using Roary (v3.11.2) with default parameters.

Roary was used to identify and classify gene clusters into:

- Core genes
- Soft-core genes
- Shell genes
- Cloud genes

The analysis also generated gene presence/absence matrices, core gene alignments, accessory genome information, and pangenome summary statistics.

### 3. Comparative Genomic Analysis

The Roary outputs were used to investigate:

- Gene conservation across the analyzed genomes.
- Distribution of core and accessory genes.
- Genome-specific gene clusters.
- Pangenome accumulation patterns.
- Core genome sequence alignment.
- Accessory gene distribution and relatedness.

## Repository Organization

### Results/Roary/

The `results/Roary/` directory contains the original outputs retained from the Roary analysis.

| File | Description |
|---|---|
| `gene_presence_absence.csv` | Annotated gene presence/absence matrix |
| `gene_presence_absence.Rtab` | Binary gene presence/absence matrix |
| `summary_statistics.txt` | Summary statistics of the pangenome |
| `core_gene_alignment.aln` | Multiple sequence alignment of core genes |
| `accessory_binary_genes.fa` | Accessory gene sequences |
| `accessory_binary_genes.fa.newick` | Accessory gene-based phylogenetic tree |
| `mytree.newick` | Newick-format tree retained with the analysis |
| `accessory.tab` | Accessory gene annotation table |
| `accessory.header.embl` | Accessory gene annotation header |
| `core_accessory.tab` | Core and accessory gene annotation table |
| `core_accessory.header.embl` | Core/accessory annotation header |
| `core_alignment_header.embl` | Core alignment annotation header |
| `blast_identity_frequency.Rtab` | BLAST identity frequency information |
| `number_of_conserved_genes.Rtab` | Distribution of conserved genes |
| `number_of_genes_in_pan_genome.Rtab` | Pangenome accumulation data |
| `number_of_new_genes.Rtab` | Number of newly identified genes |
| `number_of_unique_genes.Rtab` | Number of unique genes |
| `pan_genome_reference.fa` | Pangenome reference sequences |
| `clustered_proteins` | Clustered protein information |
| `accessory_graph` | Accessory genome visualization output |
| `core_accessory_graph` | Core/accessory genome visualization output |

## Software and Versions

| Software | Version | Purpose |
|---|---|---|
| Prokka | 1.14.6 | Prokaryotic genome annotation |
| Roary | 3.11.2 | Comparative pangenome analysis |
| BV-BRC | As accessed | Reference genome retrieval |

## Data Availability

The available Roary output files are deposited in this repository to support transparency and facilitate further comparative genomic investigations.

Reference genome sequences were retrieved from BV-BRC. The original genome records can be accessed through the corresponding database entries.

## Reproducibility and Code Availability

The original computational workflow involved genome annotation using Prokka followed by comparative pangenome analysis using Roary.

The original command-line scripts were not archived during the initial analysis. Therefore, the repository currently provides the retained computational outputs and documentation of the analytical workflow. Any subsequently reconstructed commands or scripts will be identified separately and should not be interpreted as original execution logs.

## References

1. Seemann, T. (2014). Prokka: Rapid prokaryotic genome annotation. *Bioinformatics*, 30(14), 2068–2069. https://doi.org/10.1093/bioinformatics/btu153

2. Page, A. J., et al. (2015). Roary: Rapid large-scale prokaryote pan genome analysis. *Bioinformatics*, 31(22), 3691–3693. https://doi.org/10.1093/bioinformatics/btv421

3. Olson, R. D., et al. (2023). Introducing the Bacterial and Viral Bioinformatics Resource Center (BV-BRC): A resource combining PATRIC, IRD and ViPR. *Nucleic Acids Research*, 51(D1), D678–D689. https://doi.org/10.1093/nar/gkac1003

## Contact

For further information regarding this dataset and associated research, please contact the corresponding author of the associated publication.