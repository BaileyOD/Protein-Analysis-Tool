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
```
## Usage
Example Inputs
```shell
>gene_1
ATGGCCATTGTAATGGGCCGCTGAAAGGGTGCCCGATAG

>protein_1
MKTAYIAKQRQISFVKSHFSRQDILDLWIYHTQGYFP
```
## Project Structure 
```powershell
project_folder/
│
├── data/
│   └── protein_example.fasta   # Input FASTA file
├── plots/                      # Generated histograms
├── protein_analysis.py         # Main script
└── README.md
```
## Example Output
```yaml
Protein ID: protein_1
Final Protein Length: 39 aa
Molecular Weight: 4512.36 Da
Isoelectric Point (pI): 6.92
Amino Acid Composition (%):
  A: 7.69%
  C: 0.00%
  D: 5.13%
  ...
```
Histogram plot
-Saved as plots/protein_1_aa_composition.png

## Future Improvments
This is a display of basic skills and not a direct project however
-ORF detection for unannotated DNA sequences
-Seconadry Structure predictions
-Exporting into CSV/Excel

## License
This project is licensed under the MIT License.

## Author
Bailey O'Donnell
https://github.com/%3Cyour-github-BaileyOD
