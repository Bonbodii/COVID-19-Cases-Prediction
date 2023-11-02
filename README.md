# COVID-19 Cases Prediction

## Objectives

- Solve a regression problem with deep neural networks (DNN).

## Task Description

### COVID-19 Cases Prediction

- Source: Delphi group @ CMU
  - A daily survey since October 2021 via Facebook.
  - Try to find out the data and use it for your training is forbidden.

### Given survey results in the past 3 days in a specific state in the U.S., then predict the percentage of new tested positive cases on the 3rd day.

## Data

### Feature

- States (35, encoded to one-hot vectors)
- COVID-like illness (5)
  - cli, ili, ...
- Behavior indicators (5)
  - wearing_mask, shop_indoors, restaurant_indoors, public_transit, ...
- Belief indicators (2)
  - belief_mask_effective, belief_distancing_effective.

- Mental indicator (2)
  - worried_catch_covid, worried_finance.
- Environmental indicators (3)
  - other_masked_public, other_distanced_public, ...
- Tested Positive Cases (1)
  - tested_positive (this is what we want to predict)

### One-hot Vector

One-hot Vectors: Vectors with only one element equal to one while others are zero. Usually used to encode discrete values.

## Evaluation Metric

- Mean Squared Error (MSE)
