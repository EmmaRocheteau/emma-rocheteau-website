---
title: "Deep Transfer Learning for Automated Diagnosis of Skin Lesions from Photographs"
authors:
- admin
- Doyoon Kim
author_notes:
- "Equal contribution"
- "Equal contribution"
date: "2021-11-18T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2021-11-18T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In *Machine Learning for Mobile Health Workshop at NeurIPS 2020*
publication_short: In *ML4MH at NeurIPS 2020*

abstract: Melanoma is not the most common form of skin cancer, but it is the most deadly. Currently, the disease is diagnosed by expert dermatologists, which is costly and requires timely access to medical treatment. Recent advances in deep learning have the potential to improve diagnostic performance, expedite urgent referrals and reduce burden on clinicians. Through smart phones, the technology could reach people who would not normally have access to such healthcare services, e.g. in remote parts of the world, due to financial constraints or in 2020, COVID-19 cancellations. To this end, we have investigated various transfer learning approaches by leveraging model parameters pre-trained on ImageNet with finetuning on melanoma detection. We compare EfficientNet, MnasNet, MobileNet, DenseNet, SqueezeNet, ShuffleNet, GoogleNet, ResNet, ResNeXt, VGG and a simple CNN with and without transfer learning. We find the mobile network, EfficientNet (with transfer learning) achieves the best mean performance with an area under the receiver operating characteristic curve (AUROC) of 0.931±0.005 and an area under the precision recall curve (AUPRC) of 0.840±0.010. This is significantly better than general practitioners (0.83±0.03 AUROC) and dermatologists (0.91±0.02 AUROC).

# Summary. An optional shortened abstract.
summary: Transfer learning with convolutional neural networks on the task of melanoma classification.

tags:
- ML4MH
featured: false

links:
- name: arXiv
  url: https://arxiv.org/abs/2011.04475
url_pdf: https://arxiv.org/pdf/2011.04475.pdf
url_poster: "media/melanoma_poster.pdf"

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

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
