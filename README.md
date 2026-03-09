# Soundmark Detection

This website provides additional data and code accompanying the article submission

Jakob Abeßer & Anna Kruspe: **Operationalizing soundmarks: A data-driven validation of uniqueness,
typicality, and salience in European cities**, submitted to *Applied Acoustics*, 2026

## Sound mapping between AudioSet and Soundscape Categories

The mapping between the 527 sound classes of the **PANN** SED model and the four soundscape categories is captured in [this file](data/class_labels_pann_soundscape_classes.csv)

## Soundmark score predictions by Llama-3.1-8B-Instruct model

[This file](data/soundmark_scores_with_metrics.csv) includes for all 52,700 (city, scene, sound) combinations the predicted soundmark score (between 0 and 1) as well as a textual justification by the model.

## Experiment reproduction

This [Jupyter notebook](SMD_experiments.ipynb) reproduces the experiments described in the paper.

Use the following commands to setup a suitable Python environment

```
conda create -n smd python=3.7.13 pip
conda activate smd
pip install -r requirements.txt
```