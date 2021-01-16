---
title: "Predicting Patient Outcomes with Graph Representation Learning"
authors:
- admin
- Catherine Tong
- Petar Veličković
- Nic Lane
- Pietro Liò
author_notes:
- "Equal contribution"
- "Equal contribution"
- ""
- ""
- ""
date: "2021-01-11T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2021-01-11T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In *The 5th International Workshop on Health Intelligence (W3PHIAI-21) and The Fifth International Workshop on Deep Learning on Graphs (DLG-AAAI'21) at AAAI 2021*
publication_short: In *W3PHIAI-21 and DLG-AAAI'21 at AAAI 2021*

abstract: Recent work on predicting patient outcomes in the Intensive Care Unit (ICU) has focused heavily on the physiological time series data, largely ignoring sparse data such as diagnoses and medications. When they are included, they are usually concatenated in the late stages of a model, which may struggle to learn from rarer disease patterns. Instead, we propose a strategy to exploit diagnoses as relational information by connecting similar patients in a graph. To this end, we propose LSTM-GNN for patient outcome prediction tasks a hybrid model combining Long Short-Term Memory networks (LSTMs) for extracting temporal features and Graph Neural Networks (GNNs) for extracting the patient neighbourhood information. We demonstrate that LSTM-GNNs outperform the LSTM-only baseline on length of stay prediction tasks on the eICU database. More generally, our results indicate that exploiting information from neighbouring patient cases using graph neural networks is a promising research direction, yielding tangible returns in supervised learning performance on Electronic Health Records.

# Summary. An optional shortened abstract.
summary: Our model, LSTM-GNN, is designed to take advantage of similarity between patients in the EHR (established using the diagnoses). First, it processes the time series data for each patient with the LSTM component, before sharing information within the neighbourhood of patients via the GNN. This is an alternative way of presenting diagnoses information (the common approach is to use an encoder in the late stages of a model). We found that using both methods together gains the best performance.

tags:
- W3PHIAI-21
- DLG-AAAI'21
featured: true

links:
- name: arXiv
  url: https://arxiv.org/abs/2101.03940
url_pdf: https://arxiv.org/pdf/2101.03940.pdf
url_code: https://github.com/EmmaRocheteau/eICU-GNN-LSTM

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
- grl

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
