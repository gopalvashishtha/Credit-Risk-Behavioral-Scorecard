# Credit-Risk-Behavioral-Scorecard
An Early Warning System on Python using Logistic Regression to predict 12-month PD for personal loans.


Problem Statement
The objective is to proactively manage the bank's existing personal loan portfolio. Instead of waiting for a customer to default, the bank needs a tool to evaluate the Probability of Default (PD) for current customers over the next 12 months.

By identifying high-risk customers early, the Credit Risk team can intervene—adjusting loan terms, restructuring repayment schedules, or offering financial counseling—to prevent a formal default and minimize Expected Credit Loss (ECL).

Target Definition
Performance Window: 12 Months (Behavioral).
Default Definition: 90+ Days Past Due (DPD).

In line with standard market definitions for personal retail loans, a "Bad" is defined as any customer who breaches the 90-day delinquency threshold during the performance window.

# The Story in the Data
I developed this scorecard using a dataset of 18,248 existing customers. The goal wasn't just to "predict," but to create an interpretable early warning tool that a Policy Manager could actually use to make decisions.

I chose a Logistic Regression model because the dependent variable is binary (Default vs. Non-Default), allowing for clear coefficient transparency.

Key Performance Highlights:

   Gini Coefficient: 53.53% (Strong discriminative power).
   
   KS Statistic: 0.4018 (Maximum separation at a 16.41% PD cut-off).
   
   Calibration (Brier Score): 0.1136 (Highly accurate probability forecasting).


 # Methodology

 I followed the industry-standard Weight of Evidence (WoE) and Logistic Regression framework. This ensures the model is not a "black box," but a transparent scoring tool suitable for banking audits.

