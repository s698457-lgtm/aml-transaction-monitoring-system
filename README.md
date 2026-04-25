# aml-transaction-monitoring-system
Transaction monitoring system to identify suspicious activity using rule-based anomaly detection
# AML Transaction Monitoring System

## Overview

This project implements a rule-based AML (Anti-Money Laundering) system to detect suspicious transactions using data analysis techniques.

## Objective

To identify potentially risky transactions by analyzing transaction value, behavior patterns, deviation from normal activity, and transaction frequency.

## Methodology

### Step 1: Data Loading

Transaction dataset is loaded and explored for analysis.

### Step 2: Feature Creation

Key indicators are created:

* High transaction value
* Behavioral context (transaction timing)
* Average transaction pattern
* Transaction frequency

### Step 3: Anomaly Detection

Transactions are evaluated using multiple conditions:

* High-value transactions
* Deviation from average behavior
* High transaction frequency

### Step 4: Final Decision

Transactions are flagged as suspicious if they satisfy one or more anomaly conditions.

## Workflow

Data Input → Feature Engineering → Pattern Analysis → Anomaly Detection → Flagging

## Output

* Suspicious transactions identified using `aml_flag`
* Distribution of flagged vs non-flagged transactions

## Note on Implementation

Intermediate steps such as feature creation do not produce direct output because they are used to build the final detection logic. The final result is represented by the `aml_flag` column.

## Technologies Used

Python, Pandas, Google Colab

## Key Learnings

* Understanding of AML transaction monitoring systems
* Importance of behavioral analysis in anomaly detection
* Role of multiple conditions in improving detection accuracy

## Future Improvements

* Use real transaction datasets
* Add user-level tracking instead of grouped data
* Implement machine learning models for anomaly detection
