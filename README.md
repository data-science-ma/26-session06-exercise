# Session 6 Exercise: Panel Data and Fixed Effects

**Course:** Data Science and Econometrics for International Business — Spring 2026

**Institution:** Europa-Universität Flensburg

**Session date:** Thursday, 28 May 2026

---

## Overview

In this exercise you apply fixed effects estimation to firm-level panel data. You will build the standard FE progression (pooled OLS → firm FE → two-way FE), interpret what each layer of controls does, and reflect on what fixed effects can and cannot handle.

The exercise is completed inside **`exercise-session06.qmd`**.

---

## Repository contents

| File | Purpose |
|------|---------|
| `exercise-session06.qmd` | The exercise — open this and work inside it |
| `data/wms_da_textbook.csv` | WMS panel data — already included, no download needed |
| `Session-06-Exercise.Rproj` | RStudio project file — open this first |

---

## Data

`wms_da_textbook.csv` is the World Management Survey (WMS) textbook dataset from Békés & Kézdi (2021). It contains manufacturing firms across multiple countries, surveyed in multiple waves between 2004 and 2015.

**The file is already included in this repository** — no download needed.

Original source: Békés, G. & Kézdi, G. (2021). *Data Analysis for Business, Economics, and Policy*. Cambridge University Press. Full dataset: <https://osf.io/t6zdp/>

Key variables used in the exercise:

| Variable | Description |
|---|---|
| `management` | Management quality score (1–5 scale) |
| `degree_nm` | Share of non-managers with a college degree |
| `emp_firm` | Number of employees |
| `firmid` | Unique firm identifier |
| `wave` | Survey wave (year) |
| `ownership` | Ownership type (founder, family, dispersed, etc.) |
| `cty` | Country code |

---

## How to work on this exercise

When you accept the assignment via GitHub Classroom, GitHub creates a personal copy of this repository under your account.

### Option A — Work locally (recommended)

1. Clone your repository to your computer
2. Open `Session-06-Exercise.Rproj` in RStudio
3. Open `exercise-session06.qmd` and work through each task
4. Render to HTML: **Ctrl/Cmd + Shift + K**
5. Commit and push your changes to GitHub

### Option B — Work in a Codespace

1. On your repository page, click **Code → Open with Codespaces → New codespace**
2. Wait for setup (~5 minutes the first time)
3. Open the project, render, commit, and push as above

---

## Required packages

```r
install.packages(c("tidyverse", "fixest", "modelsummary", "flextable"))
```

---

## Getting help

Post questions in the [course discussion space](https://github.com/data-science-ma/AdvancedDataScience26-Material/discussions). Helping each other is encouraged; sharing complete code solutions is not.
