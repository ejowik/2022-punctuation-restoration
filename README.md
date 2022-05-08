## Project Overview
The methodology for working on the solution involves incremental development of deliverables and summarizing progress during 3 milestones. This is because there are strong dependencies between the components of the project. The requirements for successive increments are as follows:
#### Milestone 1.:
1. Literature overview
2. Exploratory Data Analysis 

The results of the work performed have been summarized in the `docs\punctuation_restoration_milestone1.pdf` file

#### Milestone 2.:
1. Reiteration of the step of exploratory data analysis aimed at identifying symbols denormalized for the Polish language and identification of recordings for which transcription data is missing.
2. Data cleaning – i.e. the elimination of symbols denormalized for the Polish language.
3. Morphological analysis of the text with the use of Morpheus2 - the main goals were to verify the correctness of data cleaning in terms of the presence of denormalized symbols in the text (also re-checking the balance of classes), analysis of morphosyntactic markers.
4. Creating a rule-based baseline model - building a dictionary and writing rules writing regex rules that will apply a dictionary approach
5. Preparation of the first version of the implementation of the proprietary approach on top of existing solutions

The codes corresponding to the individual requirements have been placed in the following locations:
1.	`notebooks/eda.ipynb` file
2.	`notebooks/feature_engineering/data_cleaning.ipynb` file
3.	`notebooks/feature_engineering/morfeusz.ipynb` file
4.	`notebooks/baseline/baseline_model.ipynb` file (alongside supporting files for data preparation and cleaning)
5.	`src/` directory

#### Milestone 3.:
1.	Pre-trained model fine tuning
2.	Preparation and application of the functions for the evaluation of the model on the test set in accordance with the requirements of the PolEval competition
3.	Models benchmarking
4.	Baseline model evaluation

## Resources:
1. https://github.com/poleval/2021-punctuation-restoration
2. https://github.com/enelpol/poleval2021-task1
3. https://github.com/xashru/punctuation-restoration/tree/master/src
