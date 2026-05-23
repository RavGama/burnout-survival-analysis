# Work-From-Home Burnout Survival Analysis

A survival analysis study modeling time-to-burnout-onset 
across 180 remote employees over 10 days, identifying which 
daily behaviors statistically accelerate burnout.

## Overview
Generic wellness tools rarely quantify which specific remote 
work behaviors drive burnout risk. This study applies a 
time-dependent Cox Proportional Hazards model to daily 
behavioral measurements, treating burnout onset as a 
time-to-event outcome.

## Methods
- Time-dependent Cox Proportional Hazards model using 
  counting-process (tstart/tstop) format to handle 
  daily-changing predictors
- Proportional hazards assumption validated via cox.zph
- Full vs. reduced model comparison to identify the most 
  parsimonious predictive model

## Key Findings
| Predictor | Hazard Ratio | Interpretation |
|---|---|---|
| Work Hours | 1.25 | Each additional hour increases burnout risk by 25% |
| Meeting Count | 1.17 | Each additional meeting increases burnout risk by 17% |
| Sleep Hours | 0.72 | Each additional hour of sleep reduces burnout risk by 28% |

## Files
- `RavienFinalProject.Rmd` — full analysis and write-up

## Tech Stack
R, survival, survminer, ggplot2, tidyverse
