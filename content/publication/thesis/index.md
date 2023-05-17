---
title: "Representation Learning for Patients in the Intensive Care Unit"
authors:
- admin
date: "2022-12-12T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2022-12-12T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["7"]

# Publication name and optional abbreviated publication name.
publication: In *University of Cambridge Thesis Repository*
publication_short: In *Apollo*

abstract: The past decade has seen accelerating interest in Artificial Intelligence (AI) in Healthcare. Data is now being generated in the form of Electronic Health Records at a scale previously unimaginable. Not only does this create opportunities for the application of AI, but it also drives innovation in the machine learning sphere. This is because health problems can present unique challenges not encountered in other domains, and clinical decision making itself can provide ingenious approaches inspiring new learning methods. The work in this thesis sits in the space between medicine and machine learning and has contributions to both domains. The broad theme is representation learning for the patient in intensive care. The eventual aim is to promote better outcomes for patients and improve the efficiency of the healthcare system. I focus in particular on predicting patient deaths and estimated dates of discharge, because they lie at the heart of the resource allocation problem in hospitals. The efficient management of hospital beds is more important than ever in the wake of staff retention crises, post-pandemic budgets and ageing populations. Specifically, in Chapter 3, I use clinical knowledge of the medical time series (namely that they are periodic signals with particular systematic biases) to improve upon the state-of-the-art in length of stay prediction (with additional investigations into mortality prediction). In Chapter 4, I am again inspired by knowledge of the clinical decision making process to propose a method using graph neural networks to leverage data from similar patients when predicting outcomes, providing important context for the predictions and interpretability opportunities. In Chapter 5, I delve further into the representation space, exploring the effect of auxiliary tasks on the performance of patient outcome models for mechanically ventilated patients. I then cluster the learned representations with the aim of discovering hidden patient phenotypes. The vision is ultimately to create robust and holistic patient representations which are suitable for deployment in the real-world.

summary: My thesis focuses on representation learning for patients in intensive care, aiming to improve patient outcomes and healthcare system efficiency. It addresses predicting patient deaths and estimated discharge dates, essential for managing hospital beds effectively. The research incorporates clinical knowledge, periodic signals, systematic biases, and graph neural networks to enhance length of stay prediction, mortality prediction, and patient outcome models for mechanically ventilated patients, with the goal of discovering hidden patient phenotypes and creating real-world deployable representations.

tags:
- thesis
featured: true

links:
- name: Apollo
  url: https://www.repository.cam.ac.uk/handle/1810/349395
url_pdf: "media/thesis.pdf"
url_slides: "media/thesis_slides.pdf"

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
