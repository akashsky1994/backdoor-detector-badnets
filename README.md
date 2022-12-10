# Backdoor Detection and Pruning for BadNets
### Content of Repo
- B_prime_2.h5 (Model with 2% Threshold)
- B_prime_4.h5 (Model with 4% Threshold)
- B_prime_10.h5 (Model with 10% Threshold)

### Instructions

## I. Data
   1. Download the validation and test datasets from [here](https://drive.google.com/drive/folders/1Rs68uH8Xqa4j6UxG53wzD0uyI8347dSq?usp=sharing) and store them under `data/` directory.
   2. The dataset contains images from YouTube Aligned Face Dataset. We retrieve 1283 individuals and split into validation and test datasets.
   3. bd_valid.h5 and bd_test.h5 contains validation and test images with sunglasses trigger respectively, that activates the backdoor for bd_net.h5. 

## I. Running the scripts
   1. Instruction to run the pruning defense is provided in step by step manner within the python notebook.
   2. The weights of b_prime models are stored in root directory.

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


