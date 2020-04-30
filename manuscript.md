---
author-meta:
- Sheng Qian
bibliography:
- content/manual-references.json
date-meta: '2020-04-30'
header-includes: '<!--

  Manubot generated metadata rendered from header-includes-template.html.

  Suggest improvements at https://github.com/manubot/manubot/blob/master/manubot/process/header-includes-template.html

  -->

  <meta name="dc.format" content="text/html" />

  <meta name="dc.title" content="Brain-ResNet" />

  <meta name="citation_title" content="Brain-ResNet" />

  <meta property="og:title" content="Brain-ResNet" />

  <meta property="twitter:title" content="Brain-ResNet" />

  <meta name="dc.date" content="2020-04-30" />

  <meta name="citation_publication_date" content="2020-04-30" />

  <meta name="dc.language" content="en-US" />

  <meta name="citation_language" content="en-US" />

  <meta name="dc.relation.ispartof" content="Manubot" />

  <meta name="dc.publisher" content="Manubot" />

  <meta name="citation_journal_title" content="Manubot" />

  <meta name="citation_technical_report_institution" content="Manubot" />

  <meta name="citation_author" content="Sheng Qian" />

  <link rel="canonical" href="https://sq-96.github.io/Brain-ResNet/" />

  <meta property="og:url" content="https://sq-96.github.io/Brain-ResNet/" />

  <meta property="twitter:url" content="https://sq-96.github.io/Brain-ResNet/" />

  <meta name="citation_fulltext_html_url" content="https://sq-96.github.io/Brain-ResNet/" />

  <meta name="citation_pdf_url" content="https://sq-96.github.io/Brain-ResNet/manuscript.pdf" />

  <link rel="alternate" type="application/pdf" href="https://sq-96.github.io/Brain-ResNet/manuscript.pdf" />

  <link rel="alternate" type="text/html" href="https://sq-96.github.io/Brain-ResNet/v/467ece2f8f7e09d18c5a55b08e4655b1cff9fa08/" />

  <meta name="manubot_html_url_versioned" content="https://sq-96.github.io/Brain-ResNet/v/467ece2f8f7e09d18c5a55b08e4655b1cff9fa08/" />

  <meta name="manubot_pdf_url_versioned" content="https://sq-96.github.io/Brain-ResNet/v/467ece2f8f7e09d18c5a55b08e4655b1cff9fa08/manuscript.pdf" />

  <meta property="og:type" content="article" />

  <meta property="twitter:card" content="summary_large_image" />

  <link rel="icon" type="image/png" sizes="192x192" href="https://manubot.org/favicon-192x192.png" />

  <link rel="mask-icon" href="https://manubot.org/safari-pinned-tab.svg" color="#ad1457" />

  <meta name="theme-color" content="#ad1457" />

  <!-- end Manubot generated metadata -->'
keywords:
- markdown
- publishing
- manubot
lang: en-US
manubot-clear-requests-cache: false
manubot-output-bibliography: output/references.json
manubot-output-citekeys: output/citations.tsv
manubot-requests-cache-path: ci/cache/requests-cache
title: Brain-ResNet
...






<small><em>
This manuscript
([permalink](https://sq-96.github.io/Brain-ResNet/v/467ece2f8f7e09d18c5a55b08e4655b1cff9fa08/))
was automatically generated
from [sq-96/Brain-ResNet@467ece2](https://github.com/sq-96/Brain-ResNet/tree/467ece2f8f7e09d18c5a55b08e4655b1cff9fa08)
on April 30, 2020.
</em></small>

## Authors



+ **Sheng Qian**<br><br>
  <small>
  </small>



## Abstract {.page_break_before}

Decoding the regulatory behavior of DNA sequences and the functional effects of noncoding variants is a preeminent challenge in understanding the mechanisms of gene regulation. This is also important for the genetics of common diseases, as most disease-associated variants are located in noncoding regions of the genome. Recently, Convolutional Neural Networks (CNNs) based methods have been developed to predict genome-wide chromatin profiles in various cellular contexts. However, these tools and resources were often trained in cell lines or bulk tissues that are not necessarily disease-related. This is particularly an issue for neuropsychiatric disorders, where the most relevant cell and tissue types are missing in the training data used by current tools.


## Introduction {.page_break_before}

Next-generation sequencing(NGS) technologies have given rise to the development of many sequencing assays such as ATAC-seq[@doi:10.1002/0471142727.mb2129s109], DNase-seq[@doi:10.1101/pdb.prot5384], ChIPseq, RNA-seq, and FIAR-seq that measure the epigenomic landscapes across many cellular contexts, including histone marks, TF binding and chromatin accessibility. These epigenomic annotations aid the characterization of noncoding genomic variants and show promises in assessing disease-associated variants and understanding the underlying transcription machinery. There has been a joint effort to survey the noncoding part of the human genome by the community, and numerous noncoding genomic sites have been statistically identified for association with complex traits. Leveraging these resources, researchers have developed machine learning models to learn features of DNA sequences that predict chromatin profiles such as protein binding sites, chromatin accessibility, histone marks and methylation of DNA sequences. Once a sequence based model is trained to predict a certain epigenomic feature, a researcher can use it to predict the likely epigenomic effect of a DNA variant. 


## Results {.page_break_before}

#### 1. Enrichment of ASoC Variants

To validate our predicion model, we first performed enrichment analysis of allele-specific open-chromatin (ASoC) variants. Genetic variants prioritized by our prediction model are expected to have large functional effects. We hypothesize that our predictions are enriched for genetic variants with some known functions. ASoC variants have been established to be functional in brain, impacting gene expresison, histone modification and DNA methylation. We obtained ASoC variants in neural progenitor cells (NPC) and glutamatergic (iN-Glut) neurons from a neuron ATAC-Seq study. We then acquired all single nucleotide variants in open chromatin regions of NPC and iN-Glut and prioritized them by our NPC and iN-Glut Brain-ResNet scores. The top 10,000 predicted genetic variants show 4 fold enrichment of ASoC variants in NPC and iN-Glut. To show the strength of our model, we also prioritized genetic variants within open chromatin regions by Functional significance (Funsig) score and CADD score. Funsig is a measure of the signficance of magnitude of predicted chromatin effect and evolutionary conservation, and CADD score is a measure of the deleteriousness of genetic variants. As shown in Fig1, our Brain-ResNet scoring significantly outperforms Funsig and CADD scoring. This gaining may arise from two apsects. First, our model uses functional genomic data from matched cell types, which could more accurately reveal the chromatin status. Second, our model uses ResNet architecture and is based on transfer learning, which could more precisely learn regulatory codes from DNA sequences. To further address the importance of matched cell types, we used Brain-ResNet scores from the other 30 cell types to prioritize genetic variants in NPC and iN-Glut. As shown in Fig2, top predictions prioritized by matched cell types generally have higher enrichment of ASoC variants.

#### 2. Sign Consistentcy

Functional genetic variants either increase or decrease intensity of a certein activity in the genome. To test if our model can precisely predict the effect size and the direction of effect, we applied our prediction model to NPC and iN-Glut ASoC variants and compared the observed allelic imbalance and the predicted difference in functional effects between reference and alternative alleles. As shown in Fig3, Our prediction model tracks the observed allelic imbalance ratio with a correlation of 0.44 and 0.40. Notably, we found 70% variants show consistent sign in observed allelic imbalace and estimated effect, which demonstrates that the prediction model accurately captures the direction of effect. 

#### 3. Evolutionary Constraint

Evolutionary constraint has shown to be useful in identifying functionally important regions. Leveraging this strategy, we calculated GERP score for top predicted variants and randomly sampled variants in 31 cell types. GERP score measures the number of substitutions "rejected" by evolutionary constraint and higehr GERP score indicates greater magnitude of evolutionary constraint. As shown in Fig4, for most cell types, our prediction model successfully prioritized genetic variants that are under higher evolutionary constraint and are more likely to have actual biological functions. 

#### 4. Purifying Selection

Because DNA variations are more likely to be deleterious than beneficial, negative selection are required to remove damaing mutations and maintain the stability of biology system. This is especially true for functionally important variants, whose change may disrupt essential biological functions. To investigate if our Brain-ResNet score could indicate functional effects, we obtained minor allele frequency from gnomAD database for all variants within peak regions of 31 chromatin profiles and plotted them against their predicted functional effects. As shown in Fig5, there is a clear negtive correlation between minor allele frequency and Brain-ResNet score. Genetic variants with larger predicted functional effects tend to have lower minor allele frequency, which indicates the acting of negtive selection. This evidence suggests that our Brain-ResNet score is a good predictor of functional importance. 



## Figures

![
**ASoC Enrichment.**
Bar plot comparing the enrichment of allele specific open chromatin variants among three groups in two cell types.
](https://github.com/sq-96/resources/raw/master/ASoC%20Enrichment.png "Square image"){#fig:ASoC Enrichment}

![
**Cell Type Check.**
Bar plot comparing the enrichment of allele specific open chromatin variants among 31 groups in two cell types.
](https://github.com/sq-96/resources/raw/master/cell%20type%20check.png "Square image"){#fig:ASoC Enrichment}

![
**GERP Score Distribution.**
Bar plot comparing the evolutionary constraint between two groups in 31 cell types.
](https://github.com/sq-96/resources/raw/master/GERP_Score.png "Square image"){#fig:GERP Score Distribution}

![
**Sign Consistency.**
Scatter plot comparing the observed allelic imbalance and the predicted difference in functional effects between reference and alternative alleles.
](https://github.com/sq-96/resources/raw/master/sign%20consistency.png "Square image"){#fig:Sign Consistency}

![
**Minor Allele Frequency.**
Scatter plot showing the negtive correlation between minor allele frequency and Brain-ResNet predicted scores.
](https://github.com/sq-96/resources/raw/master/AF%20vs%20Score.png "Square image"){#fig:Minor Allele Frequency}

![
**Heatmap.**
Heatmap showing functional effects of credible set SNPs in 31 cell types.
](https://github.com/sq-96/resources/raw/master/heatmap_col_norm.png "Square image"){#fig:Heatmap}

![
**Tracks.**
Scatter plot showing pvalue, pip and functional effects of the candidate SNP.
](https://github.com/sq-96/resources/raw/master/rs13261217_CSMD1.png "Square image"){#fig:Heatmap}



## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>
