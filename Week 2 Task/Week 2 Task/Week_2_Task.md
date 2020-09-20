# Week 2 Task: Principal Component Analysis

# **Introduction**

You have been hired by a pharmaceutical company to analyze an RNA-Seq study they have recently conducted. The study involves treatment of pancreatic islet cells with a new experimental drug for treatment of type 2 diabetes. The company wants to investigate how the drug affects cellular mRNA levels in general, and whether the expression of key groups of genes are affected. But before that it is important to perform an exploratory data analysis to gain insight into what the dataset is.

As the patent for the new experimental drug is still pending, the company has censored the names of genes.

You have been supplied with 4 files:

- `studyDesign.tsv`: File describing treatment of the 18 samples included in the study.
- `countMatrix.tsv`: Number of RNA-Seq reads mapping to each of the genes.
- `normalizedMatrix.tsv`: normalised expression to each of the genes.
- `diabetesGene.tsv`: Collection of genes known to be involved in type 2 diabetes.

### 1. **Exploratory Data Analysis**

**Question 1.1: Read all dataset into R, and make sure all three files have matching numbers and names of both samples and genes.**

Next, we want to see if the data makes sense, by making a heat map and a PCA plot.

**Question 1.2: PCA: Using the normalized matrix, perform a Principal Components Analysis (PCA) on the samples and produce a PCA-plot of the two first components, where the axis labels show the amount of variance explained by each component and samples are colored by their experimental group. Find a way to label the samples, so the identity (the sample name) of each point can easily be seen (hint: look at geom_text() or the ggrepel package!). Note, you should center but not scale the data. Comment on your plot**

**Question 1.3: Based on the previous question, discuss (max 50 words) whether your observations indicate that there are any problems with the data - e.g. outliers, mix ups, sub-groups. If you identified problems try to fix them (e.g. remove clear outliers if you find them, fix mix-ups, etc ). If you make a correction, make a PCA plot with your corrected data to check that the correction is doing the right thing.**

**TIP:** Use ***library(tidyverse)*** in R  

Your final PCA Plot should look like this, after removal of mix-ups and outliers, where PC1 and PC2 are able to cluster the Control and Treatment groups.

![Week%202%20Task%20Principal%20Component%20Analysis%20c15462de163e4b8fb3493985787d4389/Untitled.png](Week%202%20Task%20Principal%20Component%20Analysis%20c15462de163e4b8fb3493985787d4389/Untitled.png)

**NOTE:** All datasets have been provided in Google drive, along with a reference markdown file in R to perform PCA.

***Happy Coding*** 🙂