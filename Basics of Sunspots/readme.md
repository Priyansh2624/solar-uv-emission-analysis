# Basics of Sunspots

## Overview

This project provides an introduction to **sunspots**, one of the most visible manifestations of magnetic activity on the Sun.

Sunspots are relatively dark, cooler regions that appear on the Sun's photosphere. They are formed by intense concentrations of magnetic fields that suppress convection and reduce the transport of heat from the solar interior to the surface.

Although they appear dark compared with the surrounding photosphere, sunspots are still extremely hot and emit a large amount of light.

---

## Objectives

The main objectives of this project are:

* To understand what sunspots are.
* To study how sunspots form.
* To understand the structure of a sunspot.
* To study the properties of sunspots.
* To understand sunspot groups and their classification.
* To investigate the relationship between sunspots and solar magnetic activity.
* To understand the connection between sunspots, solar flares, and other solar phenomena.

---

## What Are Sunspots?

A **sunspot** is a temporary region on the Sun's photosphere that appears darker than its surroundings because it has a lower temperature.

Sunspots are associated with strong magnetic fields, typically much stronger than the average magnetic field at the solar surface.

They generally appear as dark regions consisting of:

* **Umbra** – the dark central region.
* **Penumbra** – the lighter, filamentary region surrounding the umbra.

### Structure of a Sunspot

```text
        Photosphere
   ┌───────────────────┐
   │                   │
   │    Penumbra       │
   │      ┌─────┐      │
   │      │Umbra│      │
   │      └─────┘      │
   │                   │
   └───────────────────┘
```

---

## Why Do Sunspots Appear Dark?

Sunspots are cooler than the surrounding photosphere.

Typical photospheric temperature:

```text
~5,500 K
```

Typical sunspot umbra temperature:

```text
~3,000–4,500 K
```

Because the sunspot is cooler, it emits less visible light and therefore appears darker when viewed against the much hotter photosphere.

The strong magnetic field inhibits convective motion, reducing the transport of heat from deeper layers of the Sun to the photosphere.

---

## Formation of Sunspots

Sunspots are closely related to the Sun's magnetic field.

The Sun rotates differentially, meaning that different parts of the Sun rotate at different angular velocities. This contributes to the stretching and twisting of magnetic field lines.

When concentrated magnetic fields emerge through the photosphere, they can form regions of strong magnetic activity that appear as sunspots.

A simplified process is:

```text
Solar interior
      │
      ▼
Magnetic field generation
      │
      ▼
Magnetic field becomes concentrated
      │
      ▼
Magnetic flux emerges through photosphere
      │
      ▼
       Sunspot
```

---

## Sunspot Groups

Sunspots frequently occur in **groups** rather than as isolated spots.

A typical sunspot group may contain:

* Leading sunspots
* Following sunspots
* Multiple smaller spots
* Regions of different magnetic polarity

The arrangement and magnetic structure of these groups provide important information about solar activity.

---

## Sunspot Magnetic Polarity

Sunspots are strongly influenced by magnetic fields.

A sunspot group generally contains regions with opposite magnetic polarities:

```text
   + + + +        - - -
   + + + +        - - -
       → Magnetic field →
```

The polarity arrangement of a sunspot group is important for understanding solar magnetic activity and is used in systems such as **Hale classification**.

---

## Sunspot Life Cycle

Sunspots are temporary structures and can evolve significantly during their lifetime.

A simplified lifecycle is:

```text
Formation
   ↓
Growth
   ↓
Maximum development
   ↓
Decay
   ↓
Disappearance
```

Individual sunspots may last for days to weeks, while larger and more complex groups can persist for longer periods.

---

## Sunspot Number

The number of sunspots varies with time.

A commonly used measure is the **Wolf sunspot number**, also called the **relative sunspot number**:

$$
R = k(10g+s)
$$

where:

* \(R\) = relative sunspot number
* \(g\) = number of sunspot groups
* \(s\) = number of individual sunspots
* \(k\) = observatory-dependent correction factor

The sunspot number is an important indicator of solar activity.

---

## Solar Cycle

Sunspot activity follows an approximately **11-year cycle**.

During a solar cycle:

```text
Solar Minimum
      ↓
Increasing activity
      ↓
Solar Maximum
      ↓
Decreasing activity
      ↓
Solar Minimum
```

During **solar maximum**, the number of sunspots generally increases.

During **solar minimum**, relatively few sunspots are observed.

The Sun's magnetic field undergoes a complete polarity cycle over approximately **22 years**, with the magnetic polarity reversing around each solar maximum.

---

## Sunspots and Solar Activity

Sunspots are associated with regions of strong magnetic activity.

Magnetically complex sunspot groups can be associated with energetic solar events such as:

* Solar flares
* Coronal mass ejections (CMEs)
* Solar energetic particles

Therefore, studying sunspots is important for understanding **space weather**.

---

## Observing Sunspots

Sunspots can be observed using:

* Solar telescopes
* Filtered optical telescopes
* Solar imaging instruments
* Space-based solar observatories

**Never observe the Sun directly through an unfiltered telescope, binoculars, or camera viewfinder.** Appropriate solar-safe filters or dedicated solar observing equipment are essential.

---

## Data Analysis

Sunspot observations can be analyzed to study:

* Sunspot number
* Sunspot area
* Sunspot group evolution
* Sunspot locations
* Magnetic polarity
* Hale classification
* Solar-cycle variation
* Relationship with solar flares

Example data:

```text
Date        Group      Area     Number of Spots
------------------------------------------------
01-01-2020  12735      120      5
02-01-2020  12735      145      7
03-01-2020  12735      180      9
```

Such observations can be used to investigate how sunspot groups evolve with time.

---

## Project Structure

```text
Sunspots/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   └── sunspot_analysis.ipynb
│
├── src/
│   └── analysis.py
│
├── results/
│   └── figures/
│
├── requirements.txt
│
└── README.md
```

---

## Applications

The study of sunspots has several applications:

* Understanding solar magnetic activity
* Studying the solar cycle
* Solar flare research
* Space-weather forecasting
* Studying the Sun's magnetic field
* Understanding solar-terrestrial interactions
* Long-term analysis of solar activity

---

## Future Work

This project can be extended to include:

* Automated sunspot detection from solar images.
* Measurement of sunspot areas.
* Tracking sunspot groups across the solar disk.
* Hale classification of sunspot groups.
* Analysis of sunspot cycles.
* Correlation of sunspot activity with solar flares.
* Machine-learning-based sunspot classification.

---

## Conclusion

Sunspots are important indicators of the Sun's magnetic activity. Their formation, structure, evolution, magnetic polarity, and variation over the solar cycle provide valuable information about the behavior of the Sun.

Studying sunspots therefore forms an important foundation for understanding **solar physics and space weather**.

---

## Author

**Priyansh Sarkar**

This project is intended for educational and research purposes.
