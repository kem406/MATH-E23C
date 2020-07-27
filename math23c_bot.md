---
layout: default
title: "math23c_bot Documentation"
permalink: /math23c_bot/
---

# math23c_bot()

## Usage

```
math23c_bot(data=NULL, t=5, bar=FALSE, dist=FALSE, perm=FALSE, table=FALSE,
            scatter=FALSE, ctree=FALSE, neuralnet=FALSE, col1=NULL, col2=NULL,
            val1=NULL, val2=NULL, N=10^4, limit=7, color=NULL, shape=NULL,
            size=NULL, log=FALSE, myf=NULL, variable=NULL, outputs=NULL,
            outIn=NULL, hidden=1, string=NULL, err="sse", lin=FALSE,
            modelMatrix=NULL)
```

## Arguments

**data** - Provide the function with your dataset csv file. If left blank, the function will prompt you to select the file in your folder.

**t** - The "time" between each step. Not necessarily 1:1 with seconds.  

**bar** - Set as TRUE if you want barplots of your data.

**dist** - Set as TRUE if you want to test the fitting of a gamma and normal distribution to every column in your data.

**perm** - Set as TRUE if you want to do a permutation test involving two columns of data.

**table** - Set as TRUE if you want contingency tables of your data.

**scatter** - Set as TRUE if you want to see a scatterplot between every two columns in your dataset, in both orders.

**ctree** - Set as TRUE if you want to make a prediction using a decision tree.

**neuralnet** - Set as TRUE if you want to make a prediction using a neural net.

**col1** - The first data column used in the permutation test.

**col2** - The second data column used in the permutation test.

**val1** - The value in col1 you want to test. Can also be c().  

**val2** - If left blank, the permutation test is done using val1 vs. everything that *isn't* val1. If val2 is given, the test is done in terms of val1 vs val2. Like val1, this value can actually be several values using c().

**N** - The number of iterations used in the sampling for the permutation test.

**limit** - This integer value limits the function to creating contingency tables using data columns with only a certain number of unique values. Useful for avoiding the creation of gigantic unreadable contingency tables.

**color** - The color parameter used in ggplot.

**shape** - The shape parameter used in ggplot.

**size** - The size parameter used in ggplot.

**log** - If TRUE, scatterplots will use logarithmic regression instead of linear regression.  

**myf** - The myf parameter used in ctree().

**variable** - The (string) name of the variable to be used in the decision tree.

**outputs** - The data column representing the outputs of the neural net will be split into n columns, with n being the number of discrete values in that column. The integers denoting the positions of these new columns in the resulting pre-processed dataset go into a c() for this argument. For example, if the output is the first dataset column and contains 9 discrete values, use c(1,2,3,4,5,6,7,8,9).

**outIn** - The formula parameter in neuralnet().

**hidden** - The hidden parameter in neuralnet().

**string** - If the output column has discrete integer values, these must be converted to strings. This parameter takes in an integer representing the position of the column in the dataset.

**err** - The err.fct parameter in neuralnet().

**lin** - The linear.output parameter in neuralnet().

**modelMatrix** - The object parameter in model.matrix(). For this parameter, use as.formula(~x+0+y<sub>1</sub>+y<sub>2</sub>+...+y<sub>n</sub>) where x is the name of the output column, and y<sub>1</sub>...y<sub>n</sub> are the names of the input columns
