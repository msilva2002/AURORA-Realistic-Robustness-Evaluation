### Evaluation Results
| Method | Targeted | Constrained | Distance | Treshold | Penalty | CA | AA | ASR | MR | AD | TR | DAASR | DAMR |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| ZerothOrderOptimization | ❌ | ❌ | 122.48 | 4.03 | 0.81 | 56.80% | 55.90% | - | 7.10% | 1.58% | 3.03 | - | 0.01% | - |
| ZerothOrderOptimization | ✅ | ❌ | 123.83 | 4.08 | 0.82 | 56.80% | 56.50% | 0.53% | 0.30% | 0.53% | 7.74 | 0.00% | 0.00% | - |
| BoundaryAttack | ✅ | ❌ | 147.35 | 4.03 | 0.81 | 56.80% | 29.20% | 88.99% | 50.50% | 48.59% | 129.68 | 0.13% | 0.07% | - |
| HopSkipJump | ✅ | ❌ | 147.36 | 4.03 | 0.81 | 56.80% | 26.30% | 100.00% | 56.30% | 53.70% | 215.18 | 0.14% | 0.08% | - |
| BoundaryAttack | ❌ | ❌ | 147.35 | 4.03 | 0.81 | 56.80% | 28.50% | - | 89.20% | 49.82% | 235.36 | - | 0.13% | - |
| HopSkipJump | ❌ | ❌ | 147.36 | 4.03 | 0.81 | 56.80% | 27.80% | - | 100.00% | 51.06% | 373.39 | - | 0.14% | - |
| CarliniWagner | ✅ | ❌ | 147.35 | 4.06 | 0.81 | 56.80% | 34.30% | 73.89% | 41.60% | 39.61% | 850.76 | 0.11% | 0.06% | - |
| CarliniWagner | ❌ | ❌ | 147.35 | 4.03 | 0.81 | 56.80% | 40.60% | - | 56.40% | 28.52% | 859.76 | - | 0.08% | - |
## Robustness Evaluation
81-100: Very robust.

61-80: Robust.

41-60: Moderately robust.

21-40: Weakly robust.

0-20: Not robust.

![images/robustness.png](images/robustness.png)

###### Robustness score: 89 - Very robust.
---

![images/robustness_worst_case.png](images/robustness_worst_case.png)

###### Robustness score worst case scenario: 82.0 - Very robust.
## ZerothOrderOptimization

#### Confusion Matrix
| Actual \ Predicted | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| 0 | 425 | 0 | 12 | 0 |
| 1 | 0 | 55 | 26 | 0 |
| 2 | 3 | 25 | 267 | 1 |
| 3 | 0 | 0 | 4 | 182 |
#### Variation between each value within the categorical features

![images/independent_categorical_feature_ZerothOrderOptimization_0.png](images/independent_categorical_feature_ZerothOrderOptimization_0.png)
---

![images/independent_categorical_feature_ZerothOrderOptimization_1.png](images/independent_categorical_feature_ZerothOrderOptimization_1.png)
---

### Comparison of Normal and Perturbed Results for Categorical Features

Original data
![images/original_category_0.png](images/original_category_0.png)

Perturbed data
![images/perturbed_category_ZerothOrderOptimization_0.png](images/perturbed_category_ZerothOrderOptimization_0.png)
---

Original data
![images/original_category_1.png](images/original_category_1.png)

Perturbed data
![images/perturbed_category_ZerothOrderOptimization_1.png](images/perturbed_category_ZerothOrderOptimization_1.png)
---

### Comparison of Normal and Perturbed Results for Numerical Features

![images/numerical_features_ZerothOrderOptimization.png](images/numerical_features_ZerothOrderOptimization.png)

## ZerothOrderOptimizationTargeted

#### Confusion Matrix
| Actual \ Predicted | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| 0 | 437 | 0 | 0 | 0 |
| 1 | 0 | 81 | 0 | 0 |
| 2 | 3 | 0 | 293 | 0 |
| 3 | 0 | 0 | 0 | 186 |
#### Variation between each value within the categorical features

![images/independent_categorical_feature_ZerothOrderOptimizationTargeted_0.png](images/independent_categorical_feature_ZerothOrderOptimizationTargeted_0.png)
---

![images/independent_categorical_feature_ZerothOrderOptimizationTargeted_1.png](images/independent_categorical_feature_ZerothOrderOptimizationTargeted_1.png)
---

### Comparison of Normal and Perturbed Results for Categorical Features

Original data
![images/original_category_0.png](images/original_category_0.png)

Perturbed data
![images/perturbed_category_ZerothOrderOptimizationTargeted_0.png](images/perturbed_category_ZerothOrderOptimizationTargeted_0.png)
---

Original data
![images/original_category_1.png](images/original_category_1.png)

Perturbed data
![images/perturbed_category_ZerothOrderOptimizationTargeted_1.png](images/perturbed_category_ZerothOrderOptimizationTargeted_1.png)
---

### Comparison of Normal and Perturbed Results for Numerical Features

![images/numerical_features_ZerothOrderOptimizationTargeted.png](images/numerical_features_ZerothOrderOptimizationTargeted.png)

## BoundaryAttackTargeted

#### Confusion Matrix
| Actual \ Predicted | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| 0 | 437 | 0 | 0 | 0 |
| 1 | 71 | 6 | 4 | 0 |
| 2 | 268 | 0 | 28 | 0 |
| 3 | 162 | 0 | 0 | 24 |
#### Variation between each value within the categorical features

![images/independent_categorical_feature_BoundaryAttackTargeted_0.png](images/independent_categorical_feature_BoundaryAttackTargeted_0.png)
---

![images/independent_categorical_feature_BoundaryAttackTargeted_1.png](images/independent_categorical_feature_BoundaryAttackTargeted_1.png)
---

### Comparison of Normal and Perturbed Results for Categorical Features

Original data
![images/original_category_0.png](images/original_category_0.png)

Perturbed data
![images/perturbed_category_BoundaryAttackTargeted_0.png](images/perturbed_category_BoundaryAttackTargeted_0.png)
---

Original data
![images/original_category_1.png](images/original_category_1.png)

Perturbed data
![images/perturbed_category_BoundaryAttackTargeted_1.png](images/perturbed_category_BoundaryAttackTargeted_1.png)
---

### Comparison of Normal and Perturbed Results for Numerical Features

![images/numerical_features_BoundaryAttackTargeted.png](images/numerical_features_BoundaryAttackTargeted.png)

## HopSkipJumpTargeted

#### Confusion Matrix
| Actual \ Predicted | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| 0 | 437 | 0 | 0 | 0 |
| 1 | 81 | 0 | 0 | 0 |
| 2 | 296 | 0 | 0 | 0 |
| 3 | 186 | 0 | 0 | 0 |
#### Variation between each value within the categorical features

![images/independent_categorical_feature_HopSkipJumpTargeted_0.png](images/independent_categorical_feature_HopSkipJumpTargeted_0.png)
---

![images/independent_categorical_feature_HopSkipJumpTargeted_1.png](images/independent_categorical_feature_HopSkipJumpTargeted_1.png)
---

### Comparison of Normal and Perturbed Results for Categorical Features

Original data
![images/original_category_0.png](images/original_category_0.png)

Perturbed data
![images/perturbed_category_HopSkipJumpTargeted_0.png](images/perturbed_category_HopSkipJumpTargeted_0.png)
---

Original data
![images/original_category_1.png](images/original_category_1.png)

Perturbed data
![images/perturbed_category_HopSkipJumpTargeted_1.png](images/perturbed_category_HopSkipJumpTargeted_1.png)
---

### Comparison of Normal and Perturbed Results for Numerical Features

![images/numerical_features_HopSkipJumpTargeted.png](images/numerical_features_HopSkipJumpTargeted.png)

## BoundaryAttack

#### Confusion Matrix
| Actual \ Predicted | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| 0 | 42 | 1 | 391 | 3 |
| 1 | 42 | 7 | 31 | 1 |
| 2 | 214 | 38 | 35 | 9 |
| 3 | 75 | 0 | 87 | 24 |
#### Variation between each value within the categorical features

![images/independent_categorical_feature_BoundaryAttack_0.png](images/independent_categorical_feature_BoundaryAttack_0.png)
---

![images/independent_categorical_feature_BoundaryAttack_1.png](images/independent_categorical_feature_BoundaryAttack_1.png)
---

### Comparison of Normal and Perturbed Results for Categorical Features

Original data
![images/original_category_0.png](images/original_category_0.png)

Perturbed data
![images/perturbed_category_BoundaryAttack_0.png](images/perturbed_category_BoundaryAttack_0.png)
---

Original data
![images/original_category_1.png](images/original_category_1.png)

Perturbed data
![images/perturbed_category_BoundaryAttack_1.png](images/perturbed_category_BoundaryAttack_1.png)
---

### Comparison of Normal and Perturbed Results for Numerical Features

![images/numerical_features_BoundaryAttack.png](images/numerical_features_BoundaryAttack.png)

## HopSkipJump

#### Confusion Matrix
| Actual \ Predicted | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| 0 | 0 | 0 | 436 | 1 |
| 1 | 48 | 0 | 33 | 0 |
| 2 | 251 | 40 | 0 | 5 |
| 3 | 55 | 0 | 131 | 0 |
#### Variation between each value within the categorical features

![images/independent_categorical_feature_HopSkipJump_0.png](images/independent_categorical_feature_HopSkipJump_0.png)
---

![images/independent_categorical_feature_HopSkipJump_1.png](images/independent_categorical_feature_HopSkipJump_1.png)
---

### Comparison of Normal and Perturbed Results for Categorical Features

Original data
![images/original_category_0.png](images/original_category_0.png)

Perturbed data
![images/perturbed_category_HopSkipJump_0.png](images/perturbed_category_HopSkipJump_0.png)
---

Original data
![images/original_category_1.png](images/original_category_1.png)

Perturbed data
![images/perturbed_category_HopSkipJump_1.png](images/perturbed_category_HopSkipJump_1.png)
---

### Comparison of Normal and Perturbed Results for Numerical Features

![images/numerical_features_HopSkipJump.png](images/numerical_features_HopSkipJump.png)

## CarliniWagnerTargeted

#### Confusion Matrix
| Actual \ Predicted | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| 0 | 437 | 0 | 0 | 0 |
| 1 | 79 | 2 | 0 | 0 |
| 2 | 259 | 0 | 37 | 0 |
| 3 | 78 | 0 | 0 | 108 |
#### Variation between each value within the categorical features

![images/independent_categorical_feature_CarliniWagnerTargeted_0.png](images/independent_categorical_feature_CarliniWagnerTargeted_0.png)
---

![images/independent_categorical_feature_CarliniWagnerTargeted_1.png](images/independent_categorical_feature_CarliniWagnerTargeted_1.png)
---

### Comparison of Normal and Perturbed Results for Categorical Features

Original data
![images/original_category_0.png](images/original_category_0.png)

Perturbed data
![images/perturbed_category_CarliniWagnerTargeted_0.png](images/perturbed_category_CarliniWagnerTargeted_0.png)
---

Original data
![images/original_category_1.png](images/original_category_1.png)

Perturbed data
![images/perturbed_category_CarliniWagnerTargeted_1.png](images/perturbed_category_CarliniWagnerTargeted_1.png)
---

### Comparison of Normal and Perturbed Results for Numerical Features

![images/numerical_features_CarliniWagnerTargeted.png](images/numerical_features_CarliniWagnerTargeted.png)

## CarliniWagner

#### Confusion Matrix
| Actual \ Predicted | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| 0 | 356 | 0 | 80 | 1 |
| 1 | 43 | 0 | 37 | 1 |
| 2 | 195 | 50 | 37 | 14 |
| 3 | 14 | 0 | 129 | 43 |
#### Variation between each value within the categorical features

![images/independent_categorical_feature_CarliniWagner_0.png](images/independent_categorical_feature_CarliniWagner_0.png)
---

![images/independent_categorical_feature_CarliniWagner_1.png](images/independent_categorical_feature_CarliniWagner_1.png)
---

### Comparison of Normal and Perturbed Results for Categorical Features

Original data
![images/original_category_0.png](images/original_category_0.png)

Perturbed data
![images/perturbed_category_CarliniWagner_0.png](images/perturbed_category_CarliniWagner_0.png)
---

Original data
![images/original_category_1.png](images/original_category_1.png)

Perturbed data
![images/perturbed_category_CarliniWagner_1.png](images/perturbed_category_CarliniWagner_1.png)
---

### Comparison of Normal and Perturbed Results for Numerical Features

![images/numerical_features_CarliniWagner.png](images/numerical_features_CarliniWagner.png)
