### Evaluation Results
| Method | Targeted | Constrained | Distance | Treshold | Penalty | CA | AA | ASR | MR | AD | TR | DAASR | DAMR |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| A2PM | ❌ | ❌ | 2.18 | 4.03 | 0.81 | 56.80% | 36.80% | - | 70.70% | 35.21% | 0.87 | - | 70.70% | - |
| A2PM | ✅ | ❌ | 2.18 | 4.03 | 0.81 | 56.80% | 28.20% | 88.99% | 53.50% | 50.35% | 0.76 | 88.99% | 53.50% | - |
| ZerothOrderOptimization | ❌ | ✅ | 0.13 | 4.03 | 0.81 | 56.80% | 57.80% | - | 3.10% | -1.76% | 3.23 | - | 3.10% | - |
| ZerothOrderOptimization | ✅ | ✅ | 0.0 | 0.0 | 0.0 | 56.80% | 56.80% | 0.00% | 0.00% | 0.00% | 7.98 | - | - | - |
| BoundaryAttack | ✅ | ✅ | 0.13 | 4.03 | 0.81 | 56.80% | 55.60% | 1.42% | 4.80% | 2.11% | 124.67 | 1.42% | 4.80% | - |
| HopSkipJump | ✅ | ✅ | 0.14 | 4.03 | 0.81 | 56.80% | 59.00% | 0.00% | 4.20% | -3.87% | 208.50 | 0.00% | 4.20% | - |
| BoundaryAttack | ❌ | ✅ | 3.15 | 4.2 | 0.84 | 56.80% | 55.20% | - | 1.60% | 2.82% | 223.99 | - | 1.60% | - |
| HopSkipJump | ❌ | ✅ | 0.0 | 0.0 | 0.0 | 56.80% | 56.80% | - | 0.00% | 0.00% | 362.91 | - | - | - |
| CarliniWagner | ✅ | ✅ | 0.13 | 4.03 | 0.81 | 56.80% | 50.70% | 13.14% | 9.10% | 10.74% | 847.88 | 13.14% | 9.10% | - |
| CarliniWagner | ❌ | ✅ | 0.13 | 4.04 | 0.81 | 56.80% | 50.80% | - | 6.60% | 10.56% | 861.33 | - | 6.60% | - |
## Robustness Evaluation
81-100: Very robust.

61-80: Robust.

41-60: Moderately robust.

21-40: Weakly robust.

0-20: Not robust.

![images/robustness.png](images/robustness.png)

###### Robustness score: 84 - Very robust.
---

![images/robustness_worst_case.png](images/robustness_worst_case.png)

###### Robustness score worst case scenario: 30.0 - Weakly robust.
## A2PM

#### Confusion Matrix
| Actual \ Predicted | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| 0 | 287 | 1 | 145 | 4 |
| 1 | 9 | 0 | 72 | 0 |
| 2 | 252 | 28 | 6 | 10 |
| 3 | 137 | 0 | 49 | 0 |
#### Variation between each value within the categorical features

![images/independent_categorical_feature_A2PM_0.png](images/independent_categorical_feature_A2PM_0.png)
---

![images/independent_categorical_feature_A2PM_1.png](images/independent_categorical_feature_A2PM_1.png)
---

### Comparison of Normal and Perturbed Results for Categorical Features

Original data
![images/original_category_0.png](images/original_category_0.png)

Perturbed data
![images/perturbed_category_A2PM_0.png](images/perturbed_category_A2PM_0.png)
---

Original data
![images/original_category_1.png](images/original_category_1.png)

Perturbed data
![images/perturbed_category_A2PM_1.png](images/perturbed_category_A2PM_1.png)
---

### Comparison of Normal and Perturbed Results for Numerical Features

![images/numerical_features_A2PM.png](images/numerical_features_A2PM.png)

## A2PMTargeted

#### Confusion Matrix
| Actual \ Predicted | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| 0 | 437 | 0 | 0 | 0 |
| 1 | 48 | 13 | 19 | 1 |
| 2 | 276 | 5 | 14 | 1 |
| 3 | 177 | 1 | 7 | 1 |
#### Variation between each value within the categorical features

![images/independent_categorical_feature_A2PMTargeted_0.png](images/independent_categorical_feature_A2PMTargeted_0.png)
---

![images/independent_categorical_feature_A2PMTargeted_1.png](images/independent_categorical_feature_A2PMTargeted_1.png)
---

### Comparison of Normal and Perturbed Results for Categorical Features

Original data
![images/original_category_0.png](images/original_category_0.png)

Perturbed data
![images/perturbed_category_A2PMTargeted_0.png](images/perturbed_category_A2PMTargeted_0.png)
---

Original data
![images/original_category_1.png](images/original_category_1.png)

Perturbed data
![images/perturbed_category_A2PMTargeted_1.png](images/perturbed_category_A2PMTargeted_1.png)
---

### Comparison of Normal and Perturbed Results for Numerical Features

![images/numerical_features_A2PMTargeted.png](images/numerical_features_A2PMTargeted.png)

## ZerothOrderOptimizationConstrained

#### Confusion Matrix
| Actual \ Predicted | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| 0 | 437 | 0 | 0 | 0 |
| 1 | 0 | 73 | 8 | 0 |
| 2 | 1 | 20 | 274 | 1 |
| 3 | 0 | 0 | 1 | 185 |
#### Variation between each value within the categorical features

![images/independent_categorical_feature_ZerothOrderOptimizationConstrained_0.png](images/independent_categorical_feature_ZerothOrderOptimizationConstrained_0.png)
---

![images/independent_categorical_feature_ZerothOrderOptimizationConstrained_1.png](images/independent_categorical_feature_ZerothOrderOptimizationConstrained_1.png)
---

### Comparison of Normal and Perturbed Results for Categorical Features

Original data
![images/original_category_0.png](images/original_category_0.png)

Perturbed data
![images/perturbed_category_ZerothOrderOptimizationConstrained_0.png](images/perturbed_category_ZerothOrderOptimizationConstrained_0.png)
---

Original data
![images/original_category_1.png](images/original_category_1.png)

Perturbed data
![images/perturbed_category_ZerothOrderOptimizationConstrained_1.png](images/perturbed_category_ZerothOrderOptimizationConstrained_1.png)
---

### Comparison of Normal and Perturbed Results for Numerical Features

![images/numerical_features_ZerothOrderOptimizationConstrained.png](images/numerical_features_ZerothOrderOptimizationConstrained.png)

## ZerothOrderOptimizationConstrainedTargeted

#### Confusion Matrix
| Actual \ Predicted | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| 0 | 437 | 0 | 0 | 0 |
| 1 | 0 | 81 | 0 | 0 |
| 2 | 0 | 0 | 296 | 0 |
| 3 | 0 | 0 | 0 | 186 |
#### Variation between each value within the categorical features

![images/independent_categorical_feature_ZerothOrderOptimizationConstrainedTargeted_0.png](images/independent_categorical_feature_ZerothOrderOptimizationConstrainedTargeted_0.png)
---

![images/independent_categorical_feature_ZerothOrderOptimizationConstrainedTargeted_1.png](images/independent_categorical_feature_ZerothOrderOptimizationConstrainedTargeted_1.png)
---

### Comparison of Normal and Perturbed Results for Categorical Features

Original data
![images/original_category_0.png](images/original_category_0.png)

Perturbed data
![images/perturbed_category_ZerothOrderOptimizationConstrainedTargeted_0.png](images/perturbed_category_ZerothOrderOptimizationConstrainedTargeted_0.png)
---

Original data
![images/original_category_1.png](images/original_category_1.png)

Perturbed data
![images/perturbed_category_ZerothOrderOptimizationConstrainedTargeted_1.png](images/perturbed_category_ZerothOrderOptimizationConstrainedTargeted_1.png)
---

### Comparison of Normal and Perturbed Results for Numerical Features

![images/numerical_features_ZerothOrderOptimizationConstrainedTargeted.png](images/numerical_features_ZerothOrderOptimizationConstrainedTargeted.png)

## BoundaryConstrainedAttackTargeted

#### Confusion Matrix
| Actual \ Predicted | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| 0 | 437 | 0 | 0 | 0 |
| 1 | 5 | 52 | 23 | 1 |
| 2 | 3 | 7 | 285 | 1 |
| 3 | 0 | 8 | 0 | 178 |
#### Variation between each value within the categorical features

![images/independent_categorical_feature_BoundaryConstrainedAttackTargeted_0.png](images/independent_categorical_feature_BoundaryConstrainedAttackTargeted_0.png)
---

![images/independent_categorical_feature_BoundaryConstrainedAttackTargeted_1.png](images/independent_categorical_feature_BoundaryConstrainedAttackTargeted_1.png)
---

### Comparison of Normal and Perturbed Results for Categorical Features

Original data
![images/original_category_0.png](images/original_category_0.png)

Perturbed data
![images/perturbed_category_BoundaryConstrainedAttackTargeted_0.png](images/perturbed_category_BoundaryConstrainedAttackTargeted_0.png)
---

Original data
![images/original_category_1.png](images/original_category_1.png)

Perturbed data
![images/perturbed_category_BoundaryConstrainedAttackTargeted_1.png](images/perturbed_category_BoundaryConstrainedAttackTargeted_1.png)
---

### Comparison of Normal and Perturbed Results for Numerical Features

![images/numerical_features_BoundaryConstrainedAttackTargeted.png](images/numerical_features_BoundaryConstrainedAttackTargeted.png)

## HopSkipJumpConstrainedTargeted

#### Confusion Matrix
| Actual \ Predicted | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| 0 | 437 | 0 | 0 | 0 |
| 1 | 0 | 79 | 1 | 1 |
| 2 | 0 | 28 | 267 | 1 |
| 3 | 0 | 5 | 6 | 175 |
#### Variation between each value within the categorical features

![images/independent_categorical_feature_HopSkipJumpConstrainedTargeted_0.png](images/independent_categorical_feature_HopSkipJumpConstrainedTargeted_0.png)
---

![images/independent_categorical_feature_HopSkipJumpConstrainedTargeted_1.png](images/independent_categorical_feature_HopSkipJumpConstrainedTargeted_1.png)
---

### Comparison of Normal and Perturbed Results for Categorical Features

Original data
![images/original_category_0.png](images/original_category_0.png)

Perturbed data
![images/perturbed_category_HopSkipJumpConstrainedTargeted_0.png](images/perturbed_category_HopSkipJumpConstrainedTargeted_0.png)
---

Original data
![images/original_category_1.png](images/original_category_1.png)

Perturbed data
![images/perturbed_category_HopSkipJumpConstrainedTargeted_1.png](images/perturbed_category_HopSkipJumpConstrainedTargeted_1.png)
---

### Comparison of Normal and Perturbed Results for Numerical Features

![images/numerical_features_HopSkipJumpConstrainedTargeted.png](images/numerical_features_HopSkipJumpConstrainedTargeted.png)

## BoundaryConstrainedAttack

#### Confusion Matrix
| Actual \ Predicted | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| 0 | 429 | 0 | 8 | 0 |
| 1 | 7 | 73 | 0 | 1 |
| 2 | 0 | 0 | 296 | 0 |
| 3 | 0 | 0 | 0 | 186 |
#### Variation between each value within the categorical features

![images/independent_categorical_feature_BoundaryConstrainedAttack_0.png](images/independent_categorical_feature_BoundaryConstrainedAttack_0.png)
---

![images/independent_categorical_feature_BoundaryConstrainedAttack_1.png](images/independent_categorical_feature_BoundaryConstrainedAttack_1.png)
---

### Comparison of Normal and Perturbed Results for Categorical Features

Original data
![images/original_category_0.png](images/original_category_0.png)

Perturbed data
![images/perturbed_category_BoundaryConstrainedAttack_0.png](images/perturbed_category_BoundaryConstrainedAttack_0.png)
---

Original data
![images/original_category_1.png](images/original_category_1.png)

Perturbed data
![images/perturbed_category_BoundaryConstrainedAttack_1.png](images/perturbed_category_BoundaryConstrainedAttack_1.png)
---

### Comparison of Normal and Perturbed Results for Numerical Features

![images/numerical_features_BoundaryConstrainedAttack.png](images/numerical_features_BoundaryConstrainedAttack.png)

## HopSkipJumpConstrained

#### Confusion Matrix
| Actual \ Predicted | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| 0 | 437 | 0 | 0 | 0 |
| 1 | 0 | 81 | 0 | 0 |
| 2 | 0 | 0 | 296 | 0 |
| 3 | 0 | 0 | 0 | 186 |
#### Variation between each value within the categorical features

![images/independent_categorical_feature_HopSkipJumpConstrained_0.png](images/independent_categorical_feature_HopSkipJumpConstrained_0.png)
---

![images/independent_categorical_feature_HopSkipJumpConstrained_1.png](images/independent_categorical_feature_HopSkipJumpConstrained_1.png)
---

### Comparison of Normal and Perturbed Results for Categorical Features

Original data
![images/original_category_0.png](images/original_category_0.png)

Perturbed data
![images/perturbed_category_HopSkipJumpConstrained_0.png](images/perturbed_category_HopSkipJumpConstrained_0.png)
---

Original data
![images/original_category_1.png](images/original_category_1.png)

Perturbed data
![images/perturbed_category_HopSkipJumpConstrained_1.png](images/perturbed_category_HopSkipJumpConstrained_1.png)
---

### Comparison of Normal and Perturbed Results for Numerical Features

![images/numerical_features_HopSkipJumpConstrained.png](images/numerical_features_HopSkipJumpConstrained.png)

## CarliniWagnerConstrainedTargeted

#### Confusion Matrix
| Actual \ Predicted | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| 0 | 437 | 0 | 0 | 0 |
| 1 | 46 | 18 | 17 | 0 |
| 2 | 28 | 0 | 268 | 0 |
| 3 | 0 | 0 | 0 | 186 |
#### Variation between each value within the categorical features

![images/independent_categorical_feature_CarliniWagnerConstrainedTargeted_0.png](images/independent_categorical_feature_CarliniWagnerConstrainedTargeted_0.png)
---

![images/independent_categorical_feature_CarliniWagnerConstrainedTargeted_1.png](images/independent_categorical_feature_CarliniWagnerConstrainedTargeted_1.png)
---

### Comparison of Normal and Perturbed Results for Categorical Features

Original data
![images/original_category_0.png](images/original_category_0.png)

Perturbed data
![images/perturbed_category_CarliniWagnerConstrainedTargeted_0.png](images/perturbed_category_CarliniWagnerConstrainedTargeted_0.png)
---

Original data
![images/original_category_1.png](images/original_category_1.png)

Perturbed data
![images/perturbed_category_CarliniWagnerConstrainedTargeted_1.png](images/perturbed_category_CarliniWagnerConstrainedTargeted_1.png)
---

### Comparison of Normal and Perturbed Results for Numerical Features

![images/numerical_features_CarliniWagnerConstrainedTargeted.png](images/numerical_features_CarliniWagnerConstrainedTargeted.png)

## CarliniWagnerConstrained

#### Confusion Matrix
| Actual \ Predicted | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| 0 | 428 | 0 | 9 | 0 |
| 1 | 28 | 45 | 8 | 0 |
| 2 | 3 | 18 | 275 | 0 |
| 3 | 0 | 0 | 0 | 186 |
#### Variation between each value within the categorical features

![images/independent_categorical_feature_CarliniWagnerConstrained_0.png](images/independent_categorical_feature_CarliniWagnerConstrained_0.png)
---

![images/independent_categorical_feature_CarliniWagnerConstrained_1.png](images/independent_categorical_feature_CarliniWagnerConstrained_1.png)
---

### Comparison of Normal and Perturbed Results for Categorical Features

Original data
![images/original_category_0.png](images/original_category_0.png)

Perturbed data
![images/perturbed_category_CarliniWagnerConstrained_0.png](images/perturbed_category_CarliniWagnerConstrained_0.png)
---

Original data
![images/original_category_1.png](images/original_category_1.png)

Perturbed data
![images/perturbed_category_CarliniWagnerConstrained_1.png](images/perturbed_category_CarliniWagnerConstrained_1.png)
---

### Comparison of Normal and Perturbed Results for Numerical Features

![images/numerical_features_CarliniWagnerConstrained.png](images/numerical_features_CarliniWagnerConstrained.png)
