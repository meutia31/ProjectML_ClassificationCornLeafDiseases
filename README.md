# ClassificationofCornLeafDiseases_UsingCNNandEnsembleClassifier
Automatic classification of corn leaf diseases based on digital images using MobileNetV2 as a feature extractor and two ensemble classifier models: Random Forest and XGBoost. This study aims to support the digital transformation of the agricultural sector in order to achieve smart agriculture and national food security. 

Classification of Corn Leaf Diseases Using CNN and Ensemble Classifiers

1. Project Description This research develops an automated classification system for corn leaf diseases based on digital images, using MobileNetV2 as a feature extractor and two ensemble classifier models: Random Forest and XGBoost. This research aims to support the digital transformation of the agricultural sector in order to realize smart agriculture and national food security. The diseases classified are: Blight, Common Rust, Gray Leaf Spot, and Healthy.

2. Pre-Processing a. Resize & RGBA Handling b. Split Dataset c. Undersampling d. CLAHE e. Gaussian Blur f. Normalization

3. Model Architecture a. Feature Extraction—MobileNetV2 Preprocessed images are processed using MobileNetV2 pre-trained on ImageNet. The classification layer is removed, resulting in an output of a feature vector containing 1,280 features per image. b. Classifier (Random Forest - XGBoost) Evaluation results: - Random Forest Accuracy (93%) - XGBoost Accuracy (94%) It can be concluded that XGBoost is the best model because it has higher accuracy compared to Random Forest.

4. Specific Findings 1. Undersampling after splitting — performed to prevent data leakage in the validation and test datasets. 2. BGR → RGB conversion in CLAHE — changing cv2.COLOR_BGR2LAB to cv2.COLOR_RGB2LAB resulted in a 1% decrease in Random Forest accuracy. 3. Inconsistencies in accuracy results — resolved by locking the global randomness seed to 42. 
