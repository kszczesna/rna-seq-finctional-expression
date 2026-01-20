# RNA-seq Functional Enrichment Analysis

This project extends a standard downstream RNA-seq differential expression
analysis with functional enrichment to interpret results at the biological
process level.

The goal is to move beyond gene-level changes and identify biological
pathways and processes overrepresented among differentially expressed genes,
reflecting an industry-style bioinformatics workflow.

---

## Project overview

The analysis follows a complete downstream RNA-seq workflow:

1. Data loading and validation (expression matrix and metadata)
2. Sample-level quality control using PCA
3. Differential expression analysis (log2 fold change and statistical testing)
4. Selection of significantly differentially expressed genes
5. Gene Ontology (GO) Biological Process enrichment analysis
6. Visualization and biological interpretation of enriched pathways

---

## Project structure

rna_seq_functional_enrichment/
│
├── data/
│ ├── expression_matrix.csv
│ ├── metadata.csv
│ └── significant_genes.csv
│
├── notebooks/
│ ├── 01_qc_and_de.ipynb
│ └── 02_functional_enrichment.ipynb
│
├── results/
│ ├── plots/
│ │ └── go_biological_process_enrichment.png
│ └── enrichment_tables/
│ └── go_biological_process_enrichment.csv
│
├── environment.yml
└── README.md


---

## Functional enrichment analysis

Gene Ontology Biological Process enrichment was performed using the Enrichr
database via the `gseapy` Python package.

Enrichment analysis identifies biological processes that are statistically
overrepresented among significantly differentially expressed genes, providing
biological context beyond individual gene-level changes.

---

## Results interpretation

The enrichment results indicate significant overrepresentation of biological
processes related to cell cycle regulation, signal transduction, and stress
response.

These findings suggest that the disease condition is associated with altered
regulation of fundamental cellular pathways, supporting downstream hypothesis
generation and biological interpretation.

---

## Tools & technologies

- Python
- pandas, numpy, scipy
- scikit-learn
- gseapy
- matplotlib
- Jupyter Notebook
- conda
- Git & GitHub

---

## Notes

This project focuses on downstream RNA-seq analysis and functional
interpretation. Simplified statistical approaches are used for demonstration
purposes while reflecting real-world industry bioinformatics workflows.

---

## Author

Karolina Szczesna
