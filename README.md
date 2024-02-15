# Exploration-of-Biomarkers-and-Immune-Microenvironment-in-Severe-Bladder-Cancer
Exploratory Analysis of Genomic Biomarkers for Invasive Bladder Cancer in R 

This repository contains files/code for Georgetown HIDS 7003 (Precision Health Informatics) Final Project. This project explores the molecular changes and identifies potential biomarkers at the invasive stage of bladder cancer in comparison to normal tissue, as well as differences in immune cells infiltrates.

Introduction: Invasive Bladder Cancer (BC), or Muscle Invasive Bladder Cancer/locally advanced bladder cancer/metastatic advanced bladder cancer, is where cancer has spread into or through the muscle layer of the bladder. One of the stages of cancer is the T or Tumor stage, which looks at how far cancer tumors have grown into the bladder. There are three T stages of muscle invasive bladder cancer:
    T2 means cancer has grown into the muscle layer of the bladder 
    T3 means cancer has grown through the muscle layer into the fatty tissue layer
    T4 means cancer has grown outside the bladder OR into the prostate, OR into the wall of the pelvis or abdomen
Currently, there’s a lot of ongoing research focused on identifying biomarkers, unraveling the complexity of the immune microenvironment, and optimizing immunotherapies to improve outcomes for patients with invasive BC. 


Steps:

1) Conducted differential gene expression analysis (in R) to generate differentiallly expressed genes (DEGs) between groups of subjects at invasive stage of BC vs. normal control.
   -Ran T-test to obtain set of DEGs

2) Conducted a systems biology level analysis of the list of DEGs (generated in step 1 and filtered on FDR < 0.0001 & fold-change <= 1.5) 
   -Using list of DEGs as an input to enrichR function

3) Performed Immuno-Oncology analysis, a new type of analysis, using CIBERSORT package – (on-line).
   -Determined top 5 types of immune cells that are most prevalent in tumor group of samples (based on average fraction) 

4) Compared results of pathway analysis and CIBERSORT analysis.
   -Found pathways that are relevant to CIBERSORT analysis
   -Generated a table with selected pathways
   -Explored relevance of findings to invasive BC
