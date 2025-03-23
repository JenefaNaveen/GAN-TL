# Datasets Repository for GAN-TL Domain-Adaptive Augmentation for Enhanced Transfer Learning

This repository contains several datasets used in our research paper titled "GAN-TL Domain-Adaptive Augmentation for Enhanced Transfer Learning". Each dataset is tailored for specific types of machine learning tasks, including regression, classification, and testing robustness against incomplete data.

## Datasets Overview

### 1. Modified California Housing Prices Dataset
Modifications Applied:

Feature Scaling: Features were standardized using the StandardScaler method in scikit-learn, transforming each feature to zero mean and unit variance.

Data Splitting: The dataset was split into training and testing sets using stratified sampling (train_test_split) to ensure balanced representation across classes.

GAN-Augmented Data: Synthetic data points were generated using a Generative Adversarial Network (GAN). GAN-generated samples closely mimic the real dataset's distribution, thereby reducing the domain gap and enhancing model generalization.
#### Description
This dataset is derived from the well-known California Housing dataset from the 1990 census. It has been modified to introduce missing values to test machine learning algorithms' robustness in handling incomplete datasets.

#### Features
- **longitude**: A measure of how far west a house is; a higher value is farther west.
- **latitude**: A measure of how far north a house is; a higher value is farther north.
- **housing_median_age**: Median age of a house within a block; a lower number is a newer building.
- **total_rooms**: Total number of rooms within a block.
- **total_bedrooms**: Total number of bedrooms within a block.
- **population**: Total number of people residing within a block.
- **households**: Total number of households, a group of people residing within a home unit, for a block.
- **median_income**: Median income for households within a block of houses (measured in tens of thousands of US Dollars).
- **median_house_value**: Median house value for households within a block (measured in US Dollars).
- **ocean_proximity**: Location of the house w.r.t ocean/sea.

#### Modifications
- Random missing values are introduced across all features at a rate of approximately 5%.

#### Download
[Modified California Housing Prices Dataset](Modified_California_Housing.csv)

### 2. Updated Dataset C

#### Description
This synthetic dataset was generated using a Generative Adversarial Network (GAN). It's designed for classification tasks, with features generated to mimic complex, real-world data patterns.

#### Features
- **Feature_1 to Feature_30**: Synthetic features generated by the GAN model, representing transformed space dimensions with no direct real-world interpretation.

#### Download
[Updated Dataset C](updated_dataset_c.csv)

### 3. Modified Wine Quality Dataset

#### Description
Based on the Wine Quality Dataset, this version is augmented to meet specific criteria for classification tasks, including introducing synthetic features.

#### Features
- **Feature_1 to Feature_20**: Engineered and synthetic features derived from original wine dataset characteristics.
- **quality**: Wine quality score (target variable).

#### Modifications
- Polynomial features and interaction terms added to expand feature set to 20 features.

#### Download
[Modified Wine Quality Dataset](Modified_Wine_Dataset.csv)

## Usage
Each dataset can be used to replicate results or train new machine learning models, as described in our research. For detailed analysis and usage, refer to the scripts available in this repository.
Due to confidentiality and ongoing research activities, certain detailed internal implementations and hyperparameter tuning strategies employed in our published paper, "Enhancing Transfer Learning through GAN-Based Domain-Adaptive Augmentation," are not explicitly disclosed within this publicly available codebase.
We encourage researchers and practitioners aiming for precise replication of our results to:
1) Refer closely to the descriptions provided in our paper for deeper insights.
2) Conduct rigorous hyperparameter tuning inspired by our outlined methods.
3) Explore additional domain-specific augmentation and GAN configurations.
## Citation
If you use these datasets, please cite our paper:
