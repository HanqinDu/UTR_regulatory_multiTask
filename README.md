

# 2019-2020 HonoursProject

#### Title:

Quantifying how Cis-regulatory elements predict multi-dimensional mRNA expression programs

#### **Description of the project:**

Gene expression is the process through which cells generate diversity and resilience to environmental changes. It consists of two steps: transcription, where an intermediate molecule (mRNA) is produced from the DNA, and translation of mRNA into protein. The rate of transcription and translation can be regulated by regulatory elements acting in both cis and trans. 3'UTR, 5'UTR, and promoter are known as powerful regulatory processes that determine the rate of mRNA synthesis and decay.

In this project, we are interested in using these cis-regulatory features to predict multidimensional output that indicates how the mRNA abundance change in multiple environmental conditions. Since our goal is to quantify the effect of different elements, we should avoid clustering and go straight from element to expression pattern. Linear models with multidimensional lasso (known as an algorithm of multi-task learning) which is already implemented in the glmnet package should be a good start. As an extension, we may apply to multiple states of mRNA processing like splicing, decay, and translation by combining multiple data sets. Finally, we can carry out a quantitative analysis of the contribution of motifs in different types of CRE and ask which regions make more of a contribution to dynamic changes in gene expression.

#### **References:**

- [Genomic expression programs in the response of yeast cells to environmental changes](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC15070/). A P Gasch, P T Spellman, C M Kao, O Carmel-Harel, M B Eisen, G Storz, D Botstein, and P O Brown. Mol Biol Cell, 2000 vol. 11 (12) pp. 4241-4257.
- Jerome Friedman, Trevor Hastie, Robert Tibshirani (2010). [Regularization Paths for Generalized Linear Models via Coordinate Descent](http://www.jstatsoft.org/v33/i01/). Journal of Statistical Software, 33(1), 1-22.



#### Code

| File                           | description                                                  |
| ------------------------------ | ------------------------------------------------------------ |
| hanqin_summary.Rmd             | The core code of the project, describes the analysis process, ideas and plotting. This summary is integrated from hanqin_visualize_data and hanqin_group_lasso. |
| hanqin_visualize_data.Rmd      | investigate data and justify the group lasso                 |
| hanqin_group_lasso.Rmd         | apply group lasso and analyse the coefficients               |
| hanqin_3UTR_data_prepare.Rmd   | preprocess 3'UTR sequence data                               |
| hanqin_modify_Gasch_column.Rmd | simplify the column name of expression level dataset         |


