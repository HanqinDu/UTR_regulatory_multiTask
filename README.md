# 2019MotifHonoursProject
  Code and resources compiled together for 2019 Honours Project and Summer Work at the Wallace Lab on predicting the effects of 3'UTRs.


## Intro

All code is to be found under /src and data under /data. Code is written in .rmd format and should be opened in RStudio.

### Files and Information (As of 05/10/19):

Three files are present in root of _/src_ which contain the primary relevant code. 

1) *create_ref_dataset.Rmd* : Creates a ref_data df containing motif frequencies and codon usage in a single df from raw sun et al data.  

2) *project_report.Rmd* : Contains most recent version of primary analysis. Performs combined linear models with step selection of motifs. Does not include glmnet anymore.

__The other two files have not been updated/cleaned recently with new format/files but should work.__

3) *combined_v1.Rmd* : Original combined honours project code using Nadal-Ribelles et al scRNAseq data and decay data from both Sun et al and Chan et al. Linear modelling is done using glmnet_selection motifs. There is no codon usage etc in this.

4) *abhi_terminatome_model.Rmd* : Contains original code for simultaneous analysis of  2013 Yamanishi et al terminatome RelFI data for all yeast genes along with Chan et al DecayRate data. For each data, it performs Multiple linear models, step selected combined models, and also glmnet selection and comparison of motifs selected in each case and union of the two. 







# 2019-2020 HonoursProject

#### Title:

Quantifying how Cis-regulatory elements predict multi-dimensional mRNA expression programs

#### **Description of the project:**

Gene expression is the process through which cells generate diversity and resilience to environmental changes. It consists of two steps: transcription, where an intermediate molecule (mRNA) is produced from the DNA, and translation of mRNA into protein. The rate of transcription and translation can be regulated by regulatory elements acting in both cis and trans. 3'UTR, 5'UTR, and promoter are known as powerful regulatory processes that determine the rate of mRNA synthesis and decay.

In this project, we are interested in using these cis-regulatory features to predict multidimensional output that indicates how the mRNA abundance change in multiple environmental conditions. Since our goal is to quantify the effect of different elements, we should avoid clustering and go straight from element to expression pattern. Linear models with multidimensional lasso (known as an algorithm of multi-task learning) which is already implemented in the glmnet package should be a good start. As an extension, we may apply to multiple states of mRNA processing like splicing, decay, and translation by combining multiple data sets. Finally, we can carry out a quantitative analysis of the contribution of motifs in different types of CRE and ask which regions make more of a contribution to dynamic changes in gene expression.

#### **References:**

- [Genomic expression programs in the response of yeast cells to environmental changes](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC15070/). A P Gasch, P T Spellman, C M Kao, O Carmel-Harel, M B Eisen, G Storz, D Botstein, and P O Brown. Mol Biol Cell, 2000 vol. 11 (12) pp. 4241-4257.
- Jerome Friedman, Trevor Hastie, Robert Tibshirani (2010). [Regularization Paths for Generalized Linear Models via Coordinate Descent](http://www.jstatsoft.org/v33/i01/). Journal of Statistical Software, 33(1), 1-22.