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

  <link rel="alternate" type="text/html" href="https://sq-96.github.io/Brain-ResNet/v/d78cfeda58f3688e5b7930e3de4516265f50541c/" />

  <meta name="manubot_html_url_versioned" content="https://sq-96.github.io/Brain-ResNet/v/d78cfeda58f3688e5b7930e3de4516265f50541c/" />

  <meta name="manubot_pdf_url_versioned" content="https://sq-96.github.io/Brain-ResNet/v/d78cfeda58f3688e5b7930e3de4516265f50541c/manuscript.pdf" />

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
([permalink](https://sq-96.github.io/Brain-ResNet/v/d78cfeda58f3688e5b7930e3de4516265f50541c/))
was automatically generated
from [sq-96/Brain-ResNet@d78cfed](https://github.com/sq-96/Brain-ResNet/tree/d78cfeda58f3688e5b7930e3de4516265f50541c)
on April 12, 2020.
</em></small>

## Authors



+ **Sheng Qian**<br><br>
  <small>
  </small>



## Abstract {.page_break_before}

Decoding the regulatory behavior of DNA sequences and the functional effects of noncoding variants is a preeminent challenge in understanding the mechanisms of gene regulation. This is also important for the genetics of common diseases, as most disease-associated variants are located in noncoding regions of the genome. Recently, Convolutional Neural Networks (CNNs) based methods have been developed to predict genome-wide chromatin profiles in various cellular contexts. However, these tools and resources were often trained in cell lines or bulk tissues that are not necessarily disease-related. This is particularly an issue for neuropsychiatric disorders, where the most relevant cell and tissue types are missing in the training data used by current tools. Here we introduce a Convolutional Residual Networks (ResNet) based architecture that trains with user-provided epigenomic profiles in specific cell types while borrowing information from an extensive compendium of publicly available chromatin profiles via transfer learning. We applied this framework to a collection of epigenomic data representing early neurodevelopment, including data from iPS cell derived neurons and fetal brain. We show that our method predicts chromatin accessibility of Induced Pluripotent Stem Cell(iPSC) derived neuronal cells with higher accuracy than previous methods. Using a list of experimentally derived chromatin accessibility variants, we show that our models can predict regulatory variants with better accuracy than publicly available noncoding variant scoring tools. We also found that with the transfer learning framework, we can recover cell-type-specific motifs from our architecture, shedding light on possible regulatory mechanisms in specific cell types. In summary, we provide a general deep transfer learning framework to train on user-provided epigenomic data, and our resources would be useful for studying neuropsychiatric diseases.


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
](https://github.com/sq-96/resources/raw/master/ASoC%20Enrichment.png "Square image"){#fig:GERP Score Distribution}



## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>
