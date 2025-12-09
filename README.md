# Protein Analysis Tool

A Python script to analyze protein sequences (or DNA sequences translated to proteins) and visualize amino acid composition. Ideal for bioinformatics, genomics, and proteomics projects.

---

## Overview

This project allows users to input FASTA files containing either DNA or protein sequences. The script automatically detects the type of sequence, translates DNA to protein if necessary, computes protein statistics, and generates visualizations of amino acid composition. It is suitable for small-scale proteomics studies, genomics pipelines, or educational purposes.

---

## Features

- Automatic detection of DNA vs. protein sequences
- Translation of DNA sequences to protein (stops at first stop codon)
- Protein statistics calculation:
  - Sequence length
  - Molecular weight (Da)
  - Isoelectric point (pI)
  - Amino acid composition (%)
- Generates histogram plots of amino acid composition
- Saves plots automatically in a `/plots` folder

---

## Requirements

- Python 3.8+
- Packages:
  - [Biopython](https://biopython.org/)
  - [Matplotlib](https://matplotlib.org/)

Install required packages using:

```bash
pip install biopython matplotlib
