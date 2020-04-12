---
author-meta:
- Sheng Qian
bibliography:
- content/manual-references.json
date-meta: '2020-04-12'
header-includes: '<!--

  Manubot generated metadata rendered from header-includes-template.html.

  Suggest improvements at https://github.com/manubot/manubot/blob/master/manubot/process/header-includes-template.html

  -->

  <meta name="dc.format" content="text/html" />

  <meta name="dc.title" content="Brain-ResNet" />

  <meta name="citation_title" content="Brain-ResNet" />

  <meta property="og:title" content="Brain-ResNet" />

  <meta property="twitter:title" content="Brain-ResNet" />

  <meta name="dc.date" content="2020-04-12" />

  <meta name="citation_publication_date" content="2020-04-12" />

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

  <link rel="alternate" type="text/html" href="https://sq-96.github.io/Brain-ResNet/v/49dfb10ce72c55c4f70e7cba147b510c0917ed6e/" />

  <meta name="manubot_html_url_versioned" content="https://sq-96.github.io/Brain-ResNet/v/49dfb10ce72c55c4f70e7cba147b510c0917ed6e/" />

  <meta name="manubot_pdf_url_versioned" content="https://sq-96.github.io/Brain-ResNet/v/49dfb10ce72c55c4f70e7cba147b510c0917ed6e/manuscript.pdf" />

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
([permalink](https://sq-96.github.io/Brain-ResNet/v/49dfb10ce72c55c4f70e7cba147b510c0917ed6e/))
was automatically generated
from [sq-96/Brain-ResNet@49dfb10](https://github.com/sq-96/Brain-ResNet/tree/49dfb10ce72c55c4f70e7cba147b510c0917ed6e)
on April 12, 2020.
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

## Citations

Citation by DOI [@doi:10.1371/journal.pcbi.1007068].
 
## Figures

![
**ASoC Enrichment.**
Loaded from the latest version of image on GitHub.
](https://github.com/sq-96/resources/raw/master/ASoC%20Enrichment.png "Square image"){#fig:ASoC Enrichment}

![
**GERP Score Distribution.**
Loaded from the latest version of image on GitHub.
](https://github.com/sq-96/resources/raw/master/GERP%20Score.png "Square image"){#fig:GERP Score Distribution}

![
**Sign Consistency.**
Loaded from the latest version of image on GitHub.
](https://github.com/sq-96/resources/blob/master/sign%20consistency.png "Square image"){#fig:Sign Consistency}

![
**Minor Allele Frequency.**
Loaded from the latest version of image on GitHub.
](https://github.com/sq-96/resources/blob/master/sign%20consistency.png "Square image"){#fig:Minor Allele Frequency}

![
**Heatmap.**
Loaded from the latest version of image on GitHub.
](https://github.com/sq-96/resources/blob/master/heatmap.png "Square image"){#fig:Heatmap)



## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>
