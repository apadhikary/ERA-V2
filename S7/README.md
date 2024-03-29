# ERA1 Session 7 Assignment

## Problem Statement

1. Your new target is:  
        1. 99.4% (this must be consistently shown in your last few epochs, and not a one-time achievement)  
        2. Less than or equal to 15 Epochs  
        3. Less than 8000 Parameters  
        4. Do this using your modular code. Every model that you make must be there in the model.py file as Model_1, Model_2, etc.  
2. Do this in exactly 3 steps  
3. Each File must have a "target, result, analysis" TEXT block (either at the start or the end)  
4. You must convince why have you decided that your target should be what you have decided it to be, and your analysis MUST be correct.  
5. Evaluation is highly subjective, and if you target anything out of the order, marks will be deducted. 
6. Explain your 3 steps using these targets, results, and analysis with links to your GitHub files (Colab files moved to GitHub).  
7. Keep Receptive field calculations handy for each of your models.  
8. If your GitHub folder structure or file_names are messy, -100.  
9. When ready, attempt SESSION 7 -Assignment Solution  


## Solution, Step 1 [Notebook](./ERA1_S7_step1.ipynb)

### Target   
- Create a Setup (dataset, data loader, train/test steps and log plots)  
- Defining simple model with Convolution block, GAP, dropout and batch normalization.

### Results
- Parameters: 6,038
- Best Train Accuracy 98.82%  
- Best Test Accuracy 99.06%  

### Analysis
- Model with 6K parameters is able to reach till 99.06% accuracy in 15 epochs.
- Model is not overfitting as training and test accuracies are closeby.

## Solution, Step 2 [Notebook](./ERA1_S7_step2.ipynb)

### Target   
- Add image augmentation w random rotation and random affine to improve the model performance.

### Results
- Parameters: 6,038
- Best Train Accuracy 98.03%  
- Best Test Accuracy 99.14%  

### Analysis
- Model with 6K parameters is able to reach till 99.14% accuracy in 15 epochs.
- Image augmentation doesn't show much improvement. It may be because of presense of dropout which effectively does similar function of regularising 


## Solution, Step 3 [Notebook](./ERA1_S7_step3.ipynb)

### Target   
- Study effect of including StepLR rate scheduler.
- Increase model capacity by increasing number of convolution layer.
- Optimize the learning rate and drop out value

### Results
- Parameters: 7,416
- Best Train Accuracy 99.04%  
- Best Test Accuracy 99.37%  

### Analysis
- Model with 7.4K parameters is cross 99.38% accuracy in 15 epochs.
- Model meets all the requirement of model size, accuracy and epoch.
- Increasing model capacity and LR rate scheduler helps meet the accuracy in 15 epochs

