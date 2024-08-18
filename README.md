## Table of Contents
1. [Phase 1](#Phase1)
2. [Usage](#usage)
3. [Features](#features)
4. [Contributing](#contributing)
5. [License](#license)
6. [Contact Information](#contact-information)
7. [Acknowledgements](#acknowledgements)

# Phase 1

## Week 4
1. Check without unique function
2. Make a loop to check series all the instance pictures (if they are in same sizes)
3. Clean and consistent, if there is missing values
4. Check the images, if its the best image in the series ID
5. Pandas dataframe, drop, fillna, mode, SMOTE



## Week 5 (cuurent week)

1. Document and possibly implement data cleaning process including imputing data for missing data and to balance the dataset.
    - Imputed and balanced the dataset with SkitLearn using SimpleImputer as strategy 'most_frequent'
    - Wrote 2 important function to compare the scenarios like after and before imputing and showed using piechart
2. Document the output architecture based upon 5*5=25 sets of 3 severity levels which can then be applied to a softmax layer that processes each of those 3 severity levels as a probability. Document how that will be transformed to a submission file. 
3. Study appropriate loss function for 1 of 3 severity levels and how to combine all 25 of them for a single study 
4. Investigate distribution of number of series per study (1, 2 or 3) and number of instances per series (1 - 15?)
5. Research techniques to handle variable number of inputs (input size) via scholar.google.com, Medium/stackoverflow/TowardsDataScience.com/etc., and other peoples’ notebooks.

### Things been Done
- Created a custom datset by keeping in mind the severity level and output architecture
- Create a pipeline to preprocess the data to labeled data from train_label_coordinates
- Mapped each condition for the specific region and level to a numerical format that a model can use from 'train_label_coordinates' and mapped it to "Normal/Mild" = 1
"Moderate" = 2, "Severe" = 4 as weights
- Assigning different weights to samples based on their conditions can help the model focus more on underrepresented or more important classes.
- Using OneHotEncoding categorize the data 
- Extract the condition for the specific spinal region and level, retract the condition value from the 'train.csv'
- Converted the extracted condition into numerical format

## Week 6
1. Using x, y coordinates to extract ROI (Region of Interest)
- One of the use case for the coordinates
2. Object Detection 
3. Nomarlize the image dataset

## Installation requirements

- Installing all the necessary requirements

```sh
pip install -r requirements.txt
```
### Download the data
- [Download Now](https://www.kaggle.com/competitions/rsna-2024-lumbar-spine-degenerative-classification/data)