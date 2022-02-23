# Explainable Graph-Based Rumour Detection

This repo is for the Explainable Graph-Based Rumour Detection project. The aim of this project is to document the process and progress of the various stages of the project.

## Objective

The primary aim of this project is to explain selected state-of-the-art graph-based rumour detection models, in particular, we aim to show how model attribution changes with the restriction of event responses in early rumour detection. To understand how model attribution differs according to architectural differences, we have selected the following models to explain: 

1. <b>Bi</b>-directional <b>G</b>raph <b>C</b>onvolution <b>N</b>etwork (Bi-GCN)
2. <b>E</b>dge-enhanced <b>B</b>ayesian <b>G</b>raph <b>C</b>onvolution <b>N</b>etwork (EBGCN)
3. <b>Cla</b>im-guided <b>Hi</b>erarchical <b>G</b>raph <b>AT</b>tention Network (ClaHi-GAT)

## Related Work

#### Graph Structural Features

CV explainability techniques can be adapted for the graph component. Images can be intepreted as lattice-shaped graphs with pixels analogous to nodes, therefore graphs can be seen as a generalisation of images. There are 3 very broad categories of explainability techniques in CV which are:

1. Gradient
2. Relevance 
3. Local functions

#### Textural Features

Textual features in current NLP explainability work mainly revolves around counterfactual generation (Word Replacement) as well as a lesser used technique being individual word contribution in accumulated features (Attention).

## Propsed Work Plan

The proposed work plan with each step and sub-steps are listed below:

1. Standardisation of data preprocessing
2. Reimplement and retrain the selected models on Twitter 15/16 and PHEME  
a. Bi-GCN  
b. EBGCN  
c. ClaHi-GAT
3. Adapt explainability techniques to be applied to the models
4. Analyse generated explanations for:  
a. Full event rumour detection  
b. Early rumour detection  
&emsp;i. Time limited (15 mins, 30 mins, 1 hour, etc.)  
&emsp;ii. Response limited (25 responses, 50 responses, 100 responses, etc.)

## Updates

#### Dataset and preprocessing

|Dataset|Tweets|Links|Unique Tweet IDs|Source Tweets/Tree|Unique %|
|-------|------|-----|----------------|------------------|--------|
|Twitter 15|598258|604825|53641|1490|8.97%|-|-|-|
|Twitter 16|347360|351623|26402|818|7.6%|-|-|-|
|PHEME-9|119419|-|-|-|-|

|Dataset|Tweets|Links|Unique Tweet IDs|Source Tweets/Tree|Unique %|
|-------|------|-----|----------------|------------------|--------|
|Twitter 15 and 16|598258|604825|53641|1490|8.97%|-|-|-|

#### Twitter 15 and 16 - RvNN GitHub Repo vs RumDect2017 Dropbox

|Dataset|RumDect2017 Tweet IDs|TD File Tweet IDs|TD File Unseen Tweet IDs|BU File Tweet IDs|BU File Unseen Tweet IDs|
|-------|---------------------|-----------------|------------------------|-----------------|------------------------|
|Twitter 15 and 16|53641|1797|508|
|Twitter 16|26402|3098||

|Train 15 Tweet IDs (nfold)|Test 15 Tweet IDs (nfold)|Train 16 Tweet IDs (nfold)|Test 16 Tweet IDs (nfold)|
|--------------------------|-------------------------|--------------------------|-------------------------|


#### 

<!-- |Missing Tweets|Missing %|Added Tweets|
|--------------|---------|------------|
|Twitter 15/16 (Shaun's Data)|72055|24393|33.85%|72113| -->
