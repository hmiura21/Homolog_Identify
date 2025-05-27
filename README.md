# 🔍 homolog_identify.sh

This repository contains a Bash script designed to identify **putative histidine kinase (HK) homologs** in a nucleotide genome and determine which genes (from a provided BED file) contain those homologs.

This extends previous functionality from the `find_homologs.sh` script by incorporating BED file parsing and Bash-only filtering (no `awk`) to associate homologous domains with annotated genes.

---

## 📘 Assignment Overview

### Objectives:
1. **Perform a BLAST-based search** to identify homologous hits of a query amino acid sequence (e.g., histidine kinase domains) against a nucleotide subject file.
2. **Map the homolog hits** to genes listed in a provided BED file using **pure Bash loops and conditionals**.
3. **Output** the names of genes that contain at least one predicted histidine kinase domain.

---

## ⚙️ Usage

```bash
./homolog_identify.sh <query.faa> <subject.fna> <annotations.bed> <output.txt>
```


## 📁 Repository Structure
- `Escherichia_coli_K12.fna`: example bacteria assembly for Escherichia coli (example query data)
- `Escherichia_coli_K12.bed`: example bacteria bed file for Escherichia coli containing gene name (example bed file)
- `Pseudomonas_aeruginosa_UCBPP-PA14.fna`: example bacteria assembly for Pseudomonas aeruginosa (example query data)
- `Pseudomonas_aeruginosa_UCBPP-PA14.fna`: example bacteria bed file for Pseudomonas aeruginosa containing gene name (example bed file)
- `Vibrio_cholerae_N16961.fna`: example bacteria assembly for Vibrio cholerae (example query data)
- `Vibrio_cholerae_N16961.fna`: example bacteria bed file for Vibrio cholerae containing gene name (example bed file)
- `Wolbachia.fna`: example bacteria assembly for Wolbachia (example query data)
- `Wolbachia.fna`: example bacteria bed file for Wolbachia containing gene name (example bed file)
- `HK_domain.faa`: sequence of histidine kinase (HK) domains from the organism Escherichia coli strain K-12 (example subject file)
- `homolog_identify.sh`: script that contains all commands


