# Causal-Inference-Customer-Churn

1. Research Objective

The primary objective was to determine the causal effect of being on a long-term contract on a customer's probability of churning. The target estimand is the Average Treatment Effect (ATE).

2. Methodology

Because contract choice is endogenous, we employed advanced causal inference methods to approximate a randomized experiment.

    Data: Telco Customer Churn dataset (2019).

Treatment: Enrollment in a long-term contract (one- or two-year).

Key Methods: Inverse Probability Weighting (IPW) and a Doubly Robust (DR) estimator.

Diagnostic Checks: We confirmed model robustness through propensity score overlap and covariate balance checks (Standardized Mean Differences, SMDs), particularly after trimming for common support.

3. Key Findings

The results indicate that long-term contracts have a significant, negative causal effect on customer churn:

    IPW Estimate (Full Sample): A long-term contract reduces the probability of churn by 21.0 percentage points (ATE = -0.2102).
    Doubly Robust (DR) Estimate: A long-term contract reduces the probability of churn by 16.5 percentage points (ATE = -0.165).


Robustness Check (Trimmed IPW): After restricting the analysis to the population with strong covariate overlap, the estimated reduction remained significant at approximately 11.6 percentage points.

These findings confirm that the lower churn rates observed among long-term contract customers are causal in nature.
