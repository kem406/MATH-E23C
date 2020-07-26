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

**col1** -

**col2** -

**val1** -

val2

N

limit

color

shape

size

log

myf

variable

outputs

outIn

hidden

string

err

lin

modelMatrix
