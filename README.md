# Backdoor Detection and Pruning for BadNets
### Content of Repo
- B_prime_2.h5 (Model with 2% Threshold)
- B_prime_4.h5 (Model with 4% Threshold)
- B_prime_10.h5 (Model with 10% Threshold)

### Instructions
Instruction to run the pruning defense is provided in step by step manner within the python notebook.

### Repaired Model
| Threshold | Channel Pruned | Clean Accuracy  | Attack Success Rate |
|-----------|----------------|-----------------|---------------------|
| 2         | 75%(45)        | 95.90           | 100.0               |
| 4         | 80%(48)        | 92.29           | 99.98               |
| 10        | 86.7%(52)      | 84.54           | 77.21               |


### Repaired Net
| Threshold | Channel Pruned | Clean Accuracy  | Attack Success Rate |
|-----------|----------------|-----------------|---------------------|
| 2         | 75%(45)        | 95.74           | 100.0               |
| 4         | 80%(48)        | 92.12           | 99.98               |
| 10        | 86.7%(52)      | 84.33           | 77.21               |


