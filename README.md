# Gene Expression Analysis: Smoking and Gender Effects

This repository contains a Jupyter Notebook that analyzes gene expression data to identify genes that respond differently to smoking in men versus women.

## Problem Statement

The goal of this analysis is to identify genes whose expression levels are affected by the interaction between smoking status and gender. We're specifically looking for genes where the combined effect of smoking and gender is different from what we'd expect if smoking and gender influenced gene expression independently.

## Methodology

1. **Two-way ANOVA**: We use a two-way Analysis of Variance (ANOVA) to test for interaction effects between smoking status and gender on gene expression levels.

2. **Null Hypothesis**: Our null hypothesis is that the effect of smoking status on gene expression is the same for both genders (i.e., no interaction effect).

3. **Alternative Hypothesis**: The alternative hypothesis is that the effect of smoking on gene expression differs between men and women.

4. **P-value Calculation**: For each gene, we calculate a p-value that represents the probability of observing such an interaction effect by chance, assuming the null hypothesis is true.

## Features

- Processes a large dataset of 41,093 genes
- Performs two-way ANOVA for each gene
- Calculates p-values for the interaction effect (Smoking Status x Gender)
- Generates a histogram of p-values to visualize the distribution of interaction effects across all genes

## Requirements

To run this notebook, you'll need:

- Python 3.x
- Jupyter Notebook
- Required Python libraries: pandas, numpy, scipy, matplotlib

## Usage

1. Clone this repository
2. Open the Jupyter Notebook file `@Jupyter Notebook.ipynb`
3. Run the cells in order to perform the analysis

## Output

The notebook provides:
- Progress updates for each processed gene
- A histogram of p-values across all genes
- Potentially, a list of genes with significant interaction effects (low p-values)

