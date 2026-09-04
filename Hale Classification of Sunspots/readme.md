# Hale Classification of Sunspots

## Overview

This project focuses on the **Hale classification of sunspots**, a system used to classify sunspot groups based on their **magnetic polarity configuration** and magnetic complexity.

Sunspots are regions of intense magnetic activity on the surface of the Sun. Their magnetic structure provides important information about solar activity and can help identify regions that are more likely to produce energetic events such as **solar flares and coronal mass ejections (CMEs)**.

The Hale classification system categorizes sunspot groups according to the arrangement and polarity of their magnetic fields.

---

## Objectives

The main objectives of this project are:

* To study the Hale classification system for sunspot groups.
* To process and analyze solar/sunspot observations.
* To identify the magnetic configuration of sunspot groups.
* To classify sunspot groups according to their Hale class.
* To investigate the relationship between sunspot magnetic complexity and solar activity.
* To develop an automated or semi-automated approach for Hale classification, where applicable.

---

## Hale Classification

The Hale classification is primarily based on the **magnetic polarity arrangement** of a sunspot group.

The major Hale magnetic classes include:

| Hale Class           | Description                                                                                                                           |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| **α (Alpha)**        | A unipolar sunspot group with a single dominant magnetic polarity.                                                                    |
| **β (Beta)**         | A bipolar group with a simple separation between opposite magnetic polarities.                                                        |
| **γ (Gamma)**        | A complex group in which opposite magnetic polarities are irregularly distributed and cannot be classified simply as a bipolar group. |
| **β-γ (Beta-Gamma)** | A bipolar group with sufficiently complex polarity distribution that no simple line can separate the opposite polarities.             |
| **δ (Delta)**        | Opposite-polarity umbrae occur within a common penumbra.                                                                              |
| **β-γ-δ**            | A highly complex group exhibiting both beta-gamma and delta characteristics.                                                          |

The **β-γ-δ** configuration is considered particularly magnetically complex and is often associated with highly active solar regions.

---

## Dataset

The project can use solar observations containing information such as:

* Sunspot group identification
* Observation date and time
* Sunspot location
* Magnetic polarity
* Magnetic field measurements
* Sunspot images or magnetograms
* Existing Hale classifications, where available

The dataset used in this project should be placed in the appropriate data directory.

Example:

```text
data/
├── raw/
├── processed/
└── labels/
```

---

## Project Structure

```text
Hale-Classification/
│
├── data/
│   ├── raw/
│   ├── processed/
│   └── labels/
│
├── notebooks/
│   └── analysis.ipynb
│
├── src/
│   ├── preprocessing.py
│   ├── feature_extraction.py
│   ├── classification.py
│   └── evaluation.py
│
├── results/
│   ├── figures/
│   └── tables/
│
├── requirements.txt
│
└── README.md
```

---

## Methodology

The general workflow of the project is:

```text
Solar Observations
        │
        ▼
Data Collection
        │
        ▼
Data Preprocessing
        │
        ▼
Sunspot Group Identification
        │
        ▼
Magnetic Polarity Analysis
        │
        ▼
Feature Extraction
        │
        ▼
Hale Classification
        │
        ▼
Classification Results
        │
        ▼
Performance Evaluation
```

### 1. Data Collection

Solar observations are collected from the selected solar observation dataset.

Depending on the dataset, the input may consist of solar images, magnetograms, or tabulated sunspot-group observations.

### 2. Data Preprocessing

The raw observations are cleaned and prepared for analysis.

Typical preprocessing steps may include:

* Removing invalid observations
* Handling missing values
* Normalizing measurements
* Cropping relevant solar regions
* Identifying sunspot groups
* Converting dates and observation times into a consistent format

### 3. Magnetic Polarity Analysis

The magnetic polarity distribution of each sunspot group is analyzed.

The relative locations and distribution of positive and negative magnetic regions are used to determine whether the group is:

* Unipolar
* Bipolar
* Complex
* Delta-type

### 4. Feature Extraction

Relevant features can be extracted from the observations, including:

* Number of magnetic polarity regions
* Positive and negative polarity areas
* Distance between opposite polarities
* Magnetic flux
* Sunspot area
* Number of umbrae
* Penumbral structure
* Polarity separation
* Magnetic complexity

### 5. Hale Classification

The extracted characteristics are used to assign a Hale class to each sunspot group.

For an automated classification system, machine-learning or image-processing techniques may be used.

Possible approaches include:

* Rule-based classification
* Image processing
* Machine learning
* Convolutional Neural Networks (CNNs)
* Feature-based classification

---

## Classification Output

The final output can contain a record for each sunspot group.

Example:

```text
Date        Group ID       Hale Class
--------------------------------------
2010-01-01  11000          β
2010-01-02  11000          β-γ
2010-01-03  11000          β-γ-δ
```

The results can then be used to study how the magnetic configuration of sunspot groups changes over time.

---

## Evaluation

If an automated classification model is developed, its performance can be evaluated using metrics such as:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion matrix

For multiclass classification, the performance of each Hale class should be evaluated separately, since some classes may occur much less frequently than others.

---

## Applications

Hale classification is useful in the study of **solar magnetic activity**.

Potential applications include:

* Solar flare prediction
* Space-weather research
* Identification of magnetically complex active regions
* Statistical studies of sunspot groups
* Analysis of solar-cycle activity
* Automated processing of solar observations

---

## Technologies

Depending on the implementation, the project may use:

* **Python**
* NumPy
* Pandas
* Matplotlib
* SciPy
* SunPy
* Astropy
* Scikit-learn
* OpenCV
* TensorFlow/PyTorch

---

## Future Work

Possible extensions of this project include:

* Automating sunspot detection from solar images.
* Automatically determining magnetic polarity.
* Developing a deep-learning model for Hale classification.
* Comparing Hale classification with other sunspot classification systems.
* Studying the relationship between Hale classes and solar flares.
* Developing a time-series analysis of sunspot magnetic evolution.
* Integrating the classification system with real-time solar observations.

---

## References

The classification methodology should be based on established literature on sunspot magnetic classification and solar active regions.

Useful resources include publications and databases from organizations such as:

* NASA
* NOAA
* ESA
* National Solar Observatory
* Solar Physics research databases

---

## Author

**Priyansh Sarkar**

This project is intended for academic/research purposes and focuses on the analysis and classification of solar sunspot groups using their magnetic characteristics.

