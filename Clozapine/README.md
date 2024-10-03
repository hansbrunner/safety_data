# Clozapine Adverse Event Analysis

This repository contains a series of notebooks that explore the **adverse events (AEs)** associated with **Clozapine**, an antipsychotic drug used primarily to treat **schizophrenia**. Using real-world data from the **FDA Adverse Event Reporting System (FAERS)**, accessed via the **OpenFDA API**, these analyses focus on uncovering **safety signals**, examining **patient demographics**, and understanding **AE patterns** through advanced data science techniques.

## Notebooks Overview

### 1. **Clozapine Adverse Event Characterization and Demographic Analysis**
In this first notebook, I explore the types of adverse events most commonly reported for Clozapine and examine how they affect different demographic groups.

**Key topics include:**
- **Characterizing reported adverse events**: Identifying the most commonly reported AEs associated with Clozapine, such as **neutropenia**, **leukopenia**, and **granulocytopenia**.
- **Demographic analysis**: Investigating whether specific patient characteristics, like **age** and **gender**, influence the likelihood of experiencing the most common AEs.

### 2. **Clozapine Adverse Event Time-to-Onset and Cumulative Risk**
This notebook focuses on understanding **when** adverse events occur after the initiation of Clozapine treatment and how the **cumulative risk** of experiencing these events evolves over time.

**Key topics include:**
- **Time-to-onset analysis**: Exploring the time it takes for specific AEs to manifest after starting Clozapine.
- **Cumulative risk analysis**: Using **Kaplan-Meier survival analysis** to assess how the likelihood of AEs increases over time

### 3. **Clozapine Adverse Event Temporal Trend Analysis**

This notebook focuses on the temporal changes in AE reporting for Clozapine. By applying **change point detection** algorithms, it identifies moments when the frequency of reported adverse events shifts. The findings from this analysis provide insights into how external factors (e.g., regulatory updates, changes in monitoring practices, and drug usage trends) impact AE reporting over time.

**Key topics include:**
- **Change point detection**: Utilizing the **Pruned Exact Linear Time (PELT)** algorithm and the **Radial Basis Function (RBF)** model, this section pinpoints significant shifts in AE reporting patterns. Change points, detected in **September 2016, December 2017, and March 2019.**

### 4. **Adverse Event Co-occurrence Patterns** *(Coming Soon)*

This notebook will hopefully cover data science techniques to uncover patterns in **AE co-occurrence**, such as **association rule mining**

### 5. **Convert AE PT to SOC Mapping for Clozapine Using ChatGPT**
In this notebook, I use **ChatGPT** to map **MedDRA Preferred Terms (PTs)** to their corresponding **System Organ Classes (SOCs)**. This mapping is crucial for standardizing AE data and ensuring that analyses are aligned with established medical taxonomies.

### 6. **Predictive Modeling of Risk Factors for Adverse Events in Clozapine Treatment** *(Comin Soon)*
In this notebook, I aim to apply predictive modeling to FDA adverse event data for Clozapine to identify key risk factors for specific adverse events. By analyzing features such as **drug type, indication, age, gender, and time on drug**, I will develop **machine learning models** to predict and uncover the most significant factors contributing to adverse outcomes, ultimately identifying high-risk patient profiles. Initially, this require cleaning and preprocessing of the FDA data, which is not very streamlined.

**Key topics include:**
- **Automating PT to SOC mapping**: Leveraging **ChatGPT** to generate accurate PT to SOC mappings and streamline the process of categorizing adverse events.
- **Dataset standardization**: Using the generated mappings to standardize AE data for use in subsequent analyses.
