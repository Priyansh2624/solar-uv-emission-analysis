# 🧲 Hale (Mount Wilson) Magnetic Classification

The **Hale (Mount Wilson) magnetic classification** describes the magnetic configuration of a solar active region based on the distribution of positive and negative magnetic polarities in its sunspots.

The classification consists of a set of **base magnetic configurations** together with the **δ (Delta) qualifier**, which identifies a particularly compact opposite-polarity configuration.

---

## 📌 The Basic Magnetic Configurations

There are three fundamental magnetic structures:

### α — Alpha

A **unipolar** sunspot group.

The region is dominated by a single magnetic polarity.

```text
        + + +
      + + + + +
        + + +
```

**Configuration:** Single polarity

---

### β — Beta

A **simple bipolar** sunspot group containing both positive and negative polarities with a clear separation between them.

```text
       + + +              - - -
     + + + + +          - - - - -
       + + +              - - -
          → polarity separation
```

**Configuration:** Simple bipolar

---

### γ — Gamma

A complex region in which positive and negative polarities are distributed so irregularly that the region cannot be classified as a simple bipolar group.

```text
       +       -
    -      +       +
       -       +
    +       -       +
```

**Configuration:** Complex / mixed polarity

---

## 🔹 βγ — Beta-Gamma

A β (bipolar) region that is sufficiently complex that **no single continuous line can separate the positive and negative polarities throughout the group**.

```text
       + +       -
    +      -  +      +
       -       +
    +      -       -
```

It still has an overall bipolar character, but the polarity distribution is too complicated for a simple β classification.

**Configuration:** Complex bipolar

---

# 🔴 δ — Delta Configuration

The **δ (Delta) configuration is different from α, β, and γ.**

Delta is a **qualifier** that can be added to another magnetic class.

A δ configuration occurs when **opposite-polarity umbrae lie within a common penumbra**, with the standard NOAA definition specifying umbrae separated by less than about 2° within one penumbra.

```text
       ┌─────────────────────┐
       │      PENUMBRA       │
       │                     │
       │     +     -         │
       │    UMBRA  UMBRA     │
       │                     │
       └─────────────────────┘
```

The important point is:

> **δ does not describe the overall bipolar/complex structure by itself. It describes the presence of opposite-polarity umbrae within a common penumbra.**

Because of this, δ is normally combined with another Hale class rather than reported alone.

---

# 🔗 Possible Hale Combinations

The δ qualifier can be attached to the appropriate base configuration.

### βδ — Beta-Delta

A generally **β (simple bipolar)** region containing one or more **δ configurations**.

```text
β  +  δ
↓     ↓
Bipolar + opposite-polarity umbrae
         in common penumbra
```

**Meaning:**

> Simple bipolar region + Delta configuration

---

### βγδ — Beta-Gamma-Delta

A **βγ complex bipolar region** that also contains one or more δ configurations.

```text
βγ  +  δ
 ↓      ↓
Complex + Delta
bipolar
```

**Meaning:**

> Complex bipolar region + Delta configuration

This is one of the most magnetically complex Hale classifications.

---

### γδ — Gamma-Delta

A **γ complex region** that also contains one or more δ configurations.

```text
γ  +  δ
↓     ↓
Complex + Delta
```

**Meaning:**

> Complex mixed-polarity region + Delta configuration

This configuration is relatively uncommon.

---

# 📊 Complete Classification

| Hale Class | Base Configuration | δ Qualifier | Description                                        |
| ---------- | ------------------ | ----------- | -------------------------------------------------- |
| **α**      | Unipolar           | No          | Single dominant polarity                           |
| **β**      | Bipolar            | No          | Simple bipolar region                              |
| **γ**      | Complex            | No          | Mixed polarities; not simply bipolar               |
| **βγ**     | Complex bipolar    | No          | Bipolar but no continuous polarity-separation line |
| **βδ**     | Bipolar            | Yes         | β region containing δ configuration                |
| **γδ**     | Complex            | Yes         | γ region containing δ configuration                |
| **βγδ**    | Complex bipolar    | Yes         | βγ region containing δ configuration               |

### ⚠️ What about δ by itself?

**δ is a magnetic qualifier rather than a normal standalone group class.**

It indicates that opposite-polarity umbrae occur within the same penumbra. In practice, it is appended to the underlying configuration:

```text
β       → βδ

βγ      → βγδ

γ       → γδ
```

This is why you will commonly encounter **βδ, βγδ, and γδ**, rather than simply "δ".

---

# 🧩 Classification Hierarchy

A useful way to understand the system is:

```text
                         HALE CLASSIFICATION
                                  │
                 ┌────────────────┴────────────────┐
                 │                                 │
          Base Configuration                δ Qualifier
                 │                                 │
       ┌─────────┼─────────┐                       │
       │         │         │                       │
       α         β         γ                      δ
                 │         │                       │
                 └────┬────┘                       │
                      │                             │
                     βγ                             │
                      │                             │
                      └──────────┬──────────────────┘
                                 │
                    ┌────────────┼────────────┐
                    │            │            │
                   βδ          γδ          βγδ
```

In simpler terms:

```text
α        → unipolar

β        → simple bipolar

γ        → complex / mixed polarity

βγ       → complex bipolar

δ        → opposite-polarity umbrae
           within a common penumbra

βδ       → β  + δ

γδ       → γ  + δ

βγδ      → βγ + δ
```

---

# 🚫 Combinations That Are Not Normally Used

Not every mathematical combination of α, β, γ and δ represents a valid Hale class.

For example:

```text
αδ   ❌
αγ   ❌
αβ   ❌
```

A δ configuration requires **opposite magnetic polarities**, so it is not naturally combined with the unipolar α class.

The standard NOAA/SWPC set therefore consists of:

```text
α
β
γ
βγ
βδ
γδ
βγδ
```

with **δ functioning as a qualifier**.

---

# 📚 Eight Configurations in the HMI Guide

A very useful reference for this project is the **Montana State University HMI Solar Magnetic Field Configuration Guide**. It shows actual **SDO/HMI continuum images and HMI magnetograms** for the different Hale configurations and explicitly covers α, β, γ, βγ, δ, βδ, βγδ and γδ.

For this project, these real HMI examples are particularly useful because they allow the classification to be related directly to the same type of observations used in our analysis.

---

# 🔬 Relevance to This Project

The Hale classification provides the **magnetic-complexity label** for each active region in our dataset.

Our analysis can therefore be represented as:

```text
NOAA Active Region
        │
        ▼
Hale Classification
        │
        ├── α
        ├── β
        ├── γ
        ├── βγ
        ├── βδ
        ├── γδ
        └── βγδ
        │
        ▼
HMI Magnetic Field
        │
        ▼
AIA 1600 Å UV Emission
        │
        ▼
Compare UV Emission
with Magnetic Complexity
```

The goal is to investigate whether the **ultraviolet emission from solar active regions varies systematically with their magnetic configuration and complexity**.

---

## 🖼️ Reference Images

The classification guide used for reference contains both **HMI continuum** and **HMI magnetogram** examples for the different configurations.

**Source:** *A Guide to Sunspot Magnetic Field Configuration — Montana State University*

The guide contains examples for all the major configurations used here, including **α, β, γ, βγ, δ, βδ, βγδ and γδ**.
