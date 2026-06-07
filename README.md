# heis-hidden-entrepreneur-intelligence-system
# Hidden Entrepreneur Intelligence System (HEIS)

HEIS is an ML-powered behavioral intelligence system designed to identify hidden entrepreneur-like cardholders using transaction data.

This project was developed for **Mastercard Data Quest 2026** by **Gradient Minds Team**.

## Live Demo

ML-powered system prototype:

https://heia-front.vercel.app

## Project Overview

Hidden entrepreneurial activity often exists inside consumer banking ecosystems. Many self-employed individuals and micro-business owners use personal cards for commercial transactions, which makes them difficult to identify through traditional banking segmentation.

HEIS helps banks and financial institutions detect consumer cardholders who show business-like behavior and convert these insights into actionable SME opportunities.

## Business Problem

Traditional banking segmentation may miss customers who behave like entrepreneurs but are officially classified as consumers. As a result, banks may lose opportunities related to:

- SME customer acquisition
- POS and e-commerce acquiring
- Business card offers
- Cross-selling potential
- Customer intelligence
- Revenue growth

## Solution

HEIS transforms transaction-level data into business intelligence by detecting hidden entrepreneur-like behavior, explaining the key behavioral signals, recommending suitable banking products, and estimating potential business impact.

The system supports decision-making for different banking teams, including executives, product managers, sales leads, risk and compliance teams, and data scientists.

## Key Features

- Hidden entrepreneur detection
- Business-likeness scoring
- Cardholder-level behavioral profiling
- Proxy learning approach
- Feature engineering from transaction data
- Opportunity band classification
- Explainable reason codes
- Product recommendation engine
- Business impact calculator
- Role-based dashboard prototype

## Methodology

This is not a standard binary classification problem because consumer cardholders are not confirmed negative cases. Some consumer cardholders may show hidden entrepreneur-like behavior.

Therefore, the project uses a proxy learning approach. Known business-like behavior is used as a reference to estimate how similar consumer cardholders are to business cardholders.

## Feature Engineering

Transaction-level data was aggregated into cardholder-level behavioral features.

Main feature groups include:

### Monetary Features
- Total transaction amount
- Average transaction amount
- Median transaction amount
- Amount per active day

### Frequency Features
- Transaction count
- Number of active days
- Transaction frequency
- Unique merchant count

### Merchant Features
- MCC diversity
- Merchant concentration
- Top category share
- Recurring-capable merchant interaction

### Payment Behavior Features
- Online transaction share
- POS transaction share
- Tokenized payment usage
- Recurring payment share

### Time-Based Features
- Business-hour transaction share
- Weekend transaction share
- Operational activity patterns

## Model Output

The model generates:

- Ranked consumer cardholders
- Business-likeness scores
- Opportunity bands
- Reason codes
- Recommended actions
- Estimated revenue and ROI potential

## System Architecture

HEIS includes the following layers:

1. Data input and processing
2. Behavioral feature engineering
3. Decision intelligence layer
4. Business recommendation layer
5. Role-based application layer
6. Feedback loop for future model improvement

## Repository Structure

```text
heis-hidden-entrepreneur-intelligence-system/
│
├── README.md
├── .gitignore
│
├── notebooks/
│   └── HEIS_final_work_Gradient_Minds_Team.ipynb
│
├── presentation/
│   └── Gradient_Minds_Team_Final_Presentation_HEIS.pptx
│
├── data/
│   └── README.md
│
└── docs/
    └── README.md
