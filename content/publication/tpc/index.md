---
title: "Temporal Pointwise Convolutional Networks for Length of Stay Prediction in the Intensive Care Unit"
authors:
- admin
- Pietro Liò
- Stephanie Hyland
date: "2021-04-08T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In *Conference on Health, Inference, and Learning 2021 (also Machine Learning for Health at NeurIPS 2020, and as an oral spotlight at Healthcare Systems, Population Health, and the Role of Health-Tech at ICML 2020)*
publication_short: In *CHIL Conference 2021 (also ML4H at NeurIPS 2020 and HSYS at ICML 2020)*

abstract: The pressure of ever-increasing patient demand and budget restrictions make hospital bed management a daily challenge for clinical staff. Most critical is the efficient allocation of resource-heavy Intensive Care Unit (ICU) beds to the patients who need life support. Central to solving this problem is knowing for how long the current set of ICU patients are likely to stay in the unit. In this work, we propose a new deep learning model based on the combination of temporal convolution and pointwise (1x1) convolution, to solve the length of stay prediction task on the eICU and MIMIC-IV critical care datasets. The model - which we refer to as Temporal Pointwise Convolution (TPC) - is specifically designed to mitigate common challenges with Electronic Health Records, such as skewness, irregular sampling and missing data. In doing so, we have achieved significant performance benefits of 18-68% (metric and dataset dependent) over the commonly used Long-Short Term Memory (LSTM) network, and the multi-head self-attention network known as the Transformer. By adding mortality prediction as a side-task, we can improve performance further still, resulting in a mean absolute deviation of 1.55 days (eICU) and 2.28 days (MIMIC-IV) on predicting remaining length of stay.

# Summary. An optional shortened abstract.
summary: Our model, Temporal Pointwise Convolution (TPC), is specifically designed to mitigate common challenges with Electronic Health Records, such as skewness, irregular sampling and missing data. We have achieved significant performance benefits of 18-68% over the Long-Short Term Memory (LSTM) network, and the Transformer.

tags:
- CHIL
- ML4H
- HSYS
featured: true

links:
- name: arXiv
  url: https://dl.acm.org/doi/10.1145/3450439.3451860
url_pdf: https://dl.acm.org/doi/pdf/10.1145/3450439.3451860
url_code: https://github.com/EmmaRocheteau/TPC-LoS-prediction
url_poster: "media/tpc_poster.pdf"
url_slides: "media/tpc_slides.pdf"
url_video: https://youtu.be/bDRbATjlUmY

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: ''
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
- tpc

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
