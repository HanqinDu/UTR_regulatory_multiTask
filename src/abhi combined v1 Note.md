

#### Load data (1-75)

1. load library and set color
2. load all raw data



#### Compare data (75-196)

1. organize data and combine to get `dr_data_both` (gene name, hife_sun, hife_kar)
2. plot R^2^
3. join to get `data_all` (dr_data_both + R^2^ + mean)
4. carry out regression on CV^2^ against `half life`



#### Motif analysis (197-395)

1. obtain motif-frequency matrix (69)
2. obtain  motif-frequency matrix (69+4)
3. plot 4 motif frequency against half life (sun+kar+single cell data)



#### LM modelling (395-757)

1. binary the motif-frequency matrix
2. perform LM (linear modeling)
3. glmnet



#### output data file (757-777)





