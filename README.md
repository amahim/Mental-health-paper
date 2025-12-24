# AI-Integrated Mental Health Support for University Students

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![IEEE Standard](https://img.shields.io/badge/Standard-IEEE-blue)](https://ieeexplore.ieee.org/Xplore/home.jsp)

This repository contains the research, datasets, and implementation architecture for a dual-study AI framework designed to enhance mental health support for university students. The project integrates **Conversational Triage (Study A)** and **Optimized Appointment Management (Study B)**.

## 📌 Project Overview

[cite_start]University students globally face significant mental health challenges, yet stigma and administrative delays often prevent timely care  [cite: 81-82, 701]. This project proposes:
- **Study A:** A fine-tuned **MentalBERT** transformer model to categorize user queries into Routine, Moderate, and Crisis levels with an accuracy target of 74–86%.
- **Study B:** A **Random Forest** predictive model to reduce appointment no-shows by 10–22% through adherence forecasting.

## 🏗️ System Architecture

The system follows a tiered architecture designed for scalability and privacy:
1. **Client Tier:** Student interface via Web/Mobile app.
2. **NLP Tier:** MentalBERT engine for intent classification and sentiment analysis.
3. **Decision Tier:** Triage logic module for severity scoring.
4. **Storage/Action Tier:** Secure encrypted database and counselor alert system for crisis escalation.



## 🛠️ Technical Implementation

### Study A: Conversational Triage
- **Model:** MentalBERT (Fine-tuned Transformer).
- **Logic:** Hierarchical risk stratification (Routine → Moderate → Crisis).
- [cite_start]**Safety:** Crisis Escalation Protocol triggered at a confidence threshold > 0.85[cite: 158].

### Study B: Appointment Optimization
- **Algorithms:** Random Forest (Primary), Gradient Boosting, Logistic Regression.
- **Accuracy:** 74.55% achieved on a validated dataset of 1,100 records.
- **Key Features:** Stress Frequency, Digital Comfort, Academic Year.

## 📊 Dataset Specifications

The research utilizes a mixed dataset approach to ensure robustness while preserving student privacy:
- **Primary Data:** Structured anonymous survey from 53 IIUC students.
- **Synthetic Data:** 1,100 statistically consistent records generated via probabilistic pattern replication.

| Variable | Key Observation | Percentage |
|----------|-----------------|------------|
| Stress Frequency | Reported "Often" or "Very Often" | 51.0% |
| Help-Seeking Gap | Never sought professional help | 72.0% |
| Digital Inclination | Preference for online consultation | 73.6% |

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- PyTorch / Transformers
- Scikit-learn
- Matplotlib / Seaborn

### Installation
```bash
git clone [https://github.com/yourusername/mental-health-ai-support.git](https://github.com/yourusername/mental-health-ai-support.git)
cd mental-health-ai-support
pip install -r requirements.txt
