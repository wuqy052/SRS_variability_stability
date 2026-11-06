# Variability and stability of autistic traits in the general population: a systematic comparison between online and in-lab samples
Author: Qianying Wu, Qianhui Hong, Na Yeon Kim, Ralph Adolphs, Lynn K. Paul, Caroline J. Charpentier

Corresponding author: Caroline J. Charpentier, Department of Psychology, University of Maryland, College Park, ccharpen@umd.edu

Questions about paper findings, collaboration: contact Caroline Charpentier (ccharpen@umd.edu) or Qianying Wu (qwu@caltech.edu)

Questions about code and source data: contact Qianying Wu (qwu@caltech.edu).

Paper link: https://doi.org/10.1017/pen.2025.10001 


## Abstract
The surge of online psychological assessments have brought the autism research community both opportunities and challenges: while they enable rapid large-scale data collection and more power to characterize individual differences, they also bring concerns about data quality, generalizability beyond online samples, and whether autistic traits can be reliably characterized with self-report measures administered online. Here we tackle these concerns by providing a systematic characterization of the autistic traits variability across individuals in a large cross-sectional dataset (N=2826) as well as its temporal reliability within individuals in a test-retest dataset (N=247), with both online and in-lab samples. We measured autistic traits using the Social Responsiveness Scale, 2nd version, Adult Self Report (SRS-2-ASR) - a tool that quantifies individual differences in autistic traits along a continuum for the general adult population. Across individuals, we found elevated SRS scores in online samples and were able to trace this effect to specific subsets of SRS items. SRS scores also covaried with internalizing symptoms, decreased with age, and were lower in women compared to other genders. Within individuals, we find moderate-to-good test-retest reliability of SRS scores over long intervals, with no difference between online and in-lab samples, suggesting robust temporal stability. We conclude that there are systematic differences in autistic traits between online and in-lab samples that are partly explained by systematic population-level differences in internalizing symptoms, particularly social anxiety. Future studies that sample across different populations should measure, control for, or stratify with respect to these factors.


## To run code and replicate

### Python environment

The analysis notebook uses Python 3.9 or newer. From the repository root, create and activate a virtual environment, then install the dependencies:

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

In VS Code, select `.venv` as the Python interpreter and notebook kernel.

### Data

From the /data/ folder:
- cross_sectional_excl.csv: clean data for running variability analysis
- test_retest_excl.csv: clean data for running stability analysis
- SRS_item_description.csv: info about what subscale / factor each SRS item belongs to

### Codebook

From the /code/ folder:
- Main_analysis_SRS_Variability_Stability.ipynb: main analysis conducted in the paper. Results saved in /results/ folder, used for making figures.
- SRS_ICC.Rmd: ICCs were calculated through R. Results saved in /results/ folder, used for making figures.

### Figure

From the /figure/ folder:
- figures.ipynb: run this to generate figures, they will be saved in /output/.