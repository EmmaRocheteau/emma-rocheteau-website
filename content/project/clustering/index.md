---
title: Mechanical Ventilation Clustering
summary: Time series models for mechanical ventilation representation, clustered to uncover hidden patient subtypes in the data.
tags:
- Deep Learning
- Healthcare
date: "2022-12-02T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption:
  focal_point: Smart

links:
- icon: github
  icon_pack: fab
  name: GitHub
  url: https://github.com/EmmaRocheteau/Mechanical-Ventilation-Clustering
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

## Motivation
The advancement of Electronic Health Records (EHRs) and machine learning have enabled a data-driven and personalised approach to healthcare. One step in this direction is to uncover patient sub-types with similar disease trajectories in a heterogeneous population. This is especially important in the context of mechanical ventilation in intensive care, where mortality is high and there is no consensus on treatment. In this work, we present an approach to clustering mechanical ventilation episodes, using a multi-task combination of supervised, self-supervised and unsupervised learning techniques. Our dynamic clustering assignment is guided to reflect the phenotype, trajectory and outcomes of the patient. Experimentation on a real-world dataset is encouraging, and we hope that this could translate into actionable insights in guiding future clinical research.

## Pre-Processing Instructions

1) To run the sql files you must have the AmsterdamUMCdb database set up: https://amsterdammedicaldatascience.nl/amsterdamumcdb.

2) Follow the instructions: https://github.com/AmsterdamUMC/AmsterdamUMCdb to ensure the correct connection configuration. 

3) Replace the amsterdam_path in `paths.json` to a convenient location in your computer, and do the same for `amsterdamUMCdb_preprocessing/create_all_tables.sql` using find and replace for 
`'/Users/emmarocheteau/PycharmProjects/Mechanical-Ventilation-Clustering/amsterdam_data/'`. Leave the extra '/' at the end.

4) In your terminal, navigate to the project directory, then type the following commands:

    ```
    psql 'dbname=amsterdam user=amsterdam options=--search_path=amsterdam'
    ```
    
    Inside the psql console:
    
    ```
    \i amsterdamUMCdb_preprocessing/create_all_tables.sql
    ```
    
    This step might take a couple of hours.
    
    To quit the psql console:
    
    ```
    \q
    ```
    
5) Then run the pre-processing scripts in your terminal. This will need to run overnight:

    ```
    python3 -m amsterdamUMCdb_preprocessing.run_all_preprocessing
    ```
    
It will create the following directory structure:
   
```bash
MIMIC_data
├── test
│   ├── data.npz
│   └── vents.txt
├── train
│   ├── data.npz
│   └── vents.txt
├── val
│   ├── data.npz
│   └── vents.txt
├── flat_features.csv
├── labels.csv
├── standardisation_limits.csv
├── timeseries.csv
├── ventilator_settings.csv
└── vents.txt

```
    
   
## Running the models
Once you have run the pre-processing steps you can run all the models in your terminal. Set the working directory to Mechanical-Ventilation-Clustering, and run the following:

```
python3 -m train_prediction_only
```

```
python3 -m train_prediction_reconstruction
```
    
Note that your experiment can be customised by using command line arguments (these can be explored in args.py).
    
Each experiment you run will create a directory within logs. The naming of the directory is based on 
the date and time that you ran the experiment (to ensure that there are no name clashes). 