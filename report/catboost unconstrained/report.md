### Evaluation Results
| Method | Targeted | Constrained | Distance | Treshold | Penalty | CA | AA | ASR | MR | AD | TR | DAASR | DAMR |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| ZerothOrderOptimization | ❌ | ❌ | 0.0 | 0.0 | 0.0 | 99.30% | 99.30% | - | 0.00% | 0.00% | 2.19 | - | - | - |
| ZerothOrderOptimization | ✅ | ❌ | 0.0 | 0.0 | 0.0 | 99.30% | 99.30% | 0.00% | 0.00% | 0.00% | 4.30 | - | - | - |
| HopSkipJump | ✅ | ❌ | 145.6 | 4.02 | 0.8 | 99.30% | 26.30% | 100.00% | 73.70% | 73.51% | 161.03 | 0.14% | 0.11% | - |
| HopSkipJump | ❌ | ❌ | 147.22 | 4.03 | 0.81 | 99.30% | 18.80% | - | 81.80% | 81.07% | 192.63 | - | 0.12% | - |
| BoundaryAttack | ✅ | ❌ | 145.6 | 4.02 | 0.8 | 99.30% | 26.30% | 100.00% | 73.70% | 73.51% | 391.75 | 0.14% | 0.11% | - |
| BoundaryAttack | ❌ | ❌ | 147.22 | 4.03 | 0.81 | 99.30% | 31.20% | - | 68.80% | 68.58% | 420.11 | - | 0.10% | - |
## Robustness Evaluation
81-100: Very robust.

61-80: Robust.

41-60: Moderately robust.

21-40: Weakly robust.

0-20: Not robust.

![images/robustness.png](images/robustness.png)

###### Robustness score: 83 - Very robust.
---

![images/robustness_worst_case.png](images/robustness_worst_case.png)

###### Robustness score worst case scenario: 73.0 - Robust.
## ZerothOrderOptimization

#### Confusion Matrix
| Actual \ Predicted | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| 0 | 263 | 0 | 0 | 0 |
| 1 | 0 | 260 | 0 | 0 |
| 2 | 0 | 0 | 428 | 0 |
| 3 | 0 | 0 | 0 | 49 |
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
| 0 | 263 | 0 | 0 | 0 |
| 1 | 0 | 260 | 0 | 0 |
| 2 | 0 | 0 | 428 | 0 |
| 3 | 0 | 0 | 0 | 49 |
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

## HopSkipJumpTargeted

#### Confusion Matrix
| Actual \ Predicted | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| 0 | 263 | 0 | 0 | 0 |
| 1 | 260 | 0 | 0 | 0 |
| 2 | 428 | 0 | 0 | 0 |
| 3 | 49 | 0 | 0 | 0 |
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

## HopSkipJump

#### Confusion Matrix
| Actual \ Predicted | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| 0 | 182 | 19 | 61 | 1 |
| 1 | 137 | 0 | 123 | 0 |
| 2 | 424 | 0 | 0 | 4 |
| 3 | 45 | 0 | 4 | 0 |
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

## BoundaryAttackTargeted

#### Confusion Matrix
| Actual \ Predicted | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| 0 | 263 | 0 | 0 | 0 |
| 1 | 260 | 0 | 0 | 0 |
| 2 | 428 | 0 | 0 | 0 |
| 3 | 49 | 0 | 0 | 0 |
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

## BoundaryAttack

#### Confusion Matrix
| Actual \ Predicted | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| 0 | 181 | 39 | 43 | 0 |
| 1 | 11 | 127 | 122 | 0 |
| 2 | 421 | 2 | 4 | 1 |
| 3 | 44 | 0 | 5 | 0 |
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
