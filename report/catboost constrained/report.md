### Evaluation Results

| Method                  | Targeted | Constrained | Distance | Treshold | Penalty | CA     | AA     | ASR    | MR     | AD     | TR     | DAASR  | DAMR   |
|:-----------------------:|:--------:|:-----------:|:--------:|:--------:|:-------:|:------:|:------:|:------:|:------:|:------:|:------:|:------:|:------:|
| A2PM                    | ❌        | ❌           | 2.05     | 4.03     | 0.81    | 99.30% | 11.30% | -      | 89.20% | 88.62% | 0.17   | -      | 89.20% |
| A2PM                    | ✅        | ❌           | 2.04     | 4.02     | 0.8     | 99.30% | 27.80% | 84.53% | 72.10% | 72.00% | 0.16   | 84.53% | 72.10% |
| ZerothOrderOptimization | ❌        | ✅           | 0.0      | 0.0      | 0.0     | 99.30% | 99.30% | -      | 0.00%  | 0.00%  | 2.24   | -      | -      |
| ZerothOrderOptimization | ✅        | ✅           | 0.0      | 0.0      | 0.0     | 99.30% | 99.30% | 0.00%  | 0.00%  | 0.00%  | 4.50   | -      | -      |
| HopSkipJump             | ✅        | ✅           | 4.0      | 4.03     | 0.81    | 99.30% | 58.80% | 48.30% | 41.40% | 40.79% | 162.92 | 48.30% | 41.40% |
| HopSkipJump             | ❌        | ✅           | 4.0      | 4.05     | 0.81    | 99.30% | 57.30% | -      | 42.90% | 42.30% | 196.44 | -      | 42.90% |
| BoundaryAttack          | ✅        | ✅           | 2.0      | 4.03     | 0.81    | 99.30% | 88.60% | 12.21% | 10.90% | 10.78% | 384.82 | 12.21% | 10.90% |
| BoundaryAttack          | ❌        | ✅           | 2.0      | 4.07     | 0.81    | 99.30% | 90.10% | -      | 9.40%  | 9.26%  | 421.89 | -      | 9.40%  |

## Robustness Evaluation

81-100: Very robust.

61-80: Robust.

41-60: Moderately robust.

21-40: Weakly robust.

0-20: Not robust.

![images/robustness.png](images/robustness.png)

###### Robustness score: 65 - Robust.

---

![images/robustness_worst_case.png](images/robustness_worst_case.png)

###### Robustness score worst case scenario: 13.0 - Not robust.

## A2PM

#### Confusion Matrix

| Actual \ Predicted | 0   | 1   | 2   | 3   |
| ------------------ | --- | --- | --- | --- |
| 0                  | 105 | 34  | 103 | 21  |
| 1                  | 50  | 2   | 208 | 0   |
| 2                  | 390 | 20  | 0   | 18  |
| 3                  | 45  | 0   | 3   | 1   |

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

| Actual \ Predicted | 0   | 1   | 2   | 3   |
| ------------------ | --- | --- | --- | --- |
| 0                  | 263 | 0   | 0   | 0   |
| 1                  | 149 | 13  | 98  | 0   |
| 2                  | 427 | 0   | 1   | 0   |
| 3                  | 47  | 0   | 0   | 2   |

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

| Actual \ Predicted | 0   | 1   | 2   | 3   |
| ------------------ | --- | --- | --- | --- |
| 0                  | 263 | 0   | 0   | 0   |
| 1                  | 0   | 260 | 0   | 0   |
| 2                  | 0   | 0   | 428 | 0   |
| 3                  | 0   | 0   | 0   | 49  |

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

| Actual \ Predicted | 0   | 1   | 2   | 3   |
| ------------------ | --- | --- | --- | --- |
| 0                  | 263 | 0   | 0   | 0   |
| 1                  | 0   | 260 | 0   | 0   |
| 2                  | 0   | 0   | 428 | 0   |
| 3                  | 0   | 0   | 0   | 49  |

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

## HopSkipJumpConstrainedTargeted

#### Confusion Matrix

| Actual \ Predicted | 0   | 1   | 2   | 3   |
| ------------------ | --- | --- | --- | --- |
| 0                  | 263 | 0   | 0   | 0   |
| 1                  | 114 | 91  | 55  | 0   |
| 2                  | 221 | 0   | 204 | 3   |
| 3                  | 21  | 0   | 0   | 28  |

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

## HopSkipJumpConstrained

#### Confusion Matrix

| Actual \ Predicted | 0   | 1   | 2   | 3   |
| ------------------ | --- | --- | --- | --- |
| 0                  | 233 | 3   | 27  | 0   |
| 1                  | 48  | 90  | 122 | 0   |
| 2                  | 199 | 2   | 223 | 4   |
| 3                  | 21  | 0   | 3   | 25  |

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

## BoundaryConstrainedAttackTargeted

#### Confusion Matrix

| Actual \ Predicted | 0   | 1   | 2   | 3   |
| ------------------ | --- | --- | --- | --- |
| 0                  | 263 | 0   | 0   | 0   |
| 1                  | 33  | 211 | 16  | 0   |
| 2                  | 49  | 0   | 379 | 0   |
| 3                  | 8   | 0   | 3   | 38  |

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

## BoundaryConstrainedAttack

#### Confusion Matrix

| Actual \ Predicted | 0   | 1   | 2   | 3   |
| ------------------ | --- | --- | --- | --- |
| 0                  | 249 | 6   | 8   | 0   |
| 1                  | 1   | 245 | 14  | 0   |
| 2                  | 48  | 1   | 378 | 1   |
| 3                  | 10  | 0   | 5   | 34  |

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
