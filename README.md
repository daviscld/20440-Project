
# 20440-Project
Class project for MIT's 20.440

## Overview
This repo contains code to reproduce the differential gene expression analysis 
heatmap from Christine D. and Bri K.'s 2-page proposal, as well as a few 
additional exploratory figures (PCA plot, volcano plot for differential gene
expression). In the future, this repository will contain all  code associated 
with the 20.440 class project.

## Data
Data used are publicly available and found in GEO, accession number GSE99480.

Original data come from:

Manni M, Gupta S, Ricker E, Chinenov Y et al. Regulation of age-associated B 
cells by IRF5 in systemic autoimmunity. Nat Immunol 2018 Apr;19(4):407-419.
DOI 10.1038/s41590-018-0056-8

Data are log2 cpm (counts/million counts) gene counts generated from flow 
cytometry-selected age-associated B cells from 2 wild-type mice and 2 mice with 
double-knock outs in the SWEF-family proteins. Data include authors' original 
differential expression results using EDGER, but this analysis is re-done using 
limma in this project.

## Folder structure
Figures generated are stored in a Figures subfolder, data are stored in the
Data subfolder, and code-associated files are stored in the Code subfolder.

## Installation
This code is an R markdown file.
Before running this file, please install the required programs and packages.

Install R and RStudio. If you use Mac OS, please also install XQuartz and Xcode.

Install the following packages:
readr
pheatmap
dendsort
viridis
ggrepel
ggplot2
dplyr
limma

Use the command install.packages(c("readr", "pheatmap", "dendsort", "viridis",
"ggrepel","ggplot2","dplyr","limma"))

Run the markdown file by clicking run in the upper righthand corner and 
selecting run all.

## Code
Code for the volcano plot visualization is modeled after Mark Dunning's 
2020 version of "Analysing Data from GEO- Work In Progress"
https://sbc.shef.ac.uk/geo_tutorial/tutorial.nb.html