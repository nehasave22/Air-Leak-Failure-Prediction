# **Predictive Maintenance of Air Production Units in Metro Transit Trains**

## **Project Overview**
This project focuses on developing machine learning models to predict air leak failures in the Air Production Unit (APU) of metro transit trains. The APU is essential for maintaining pneumatic pressure, and its failure can lead to costly service interruptions. By leveraging predictive analytics, this project enables proactive maintenance strategies to reduce downtime and optimize operational efficiency.

## **Dataset**
- The dataset consists of **1,516,948** sensor readings collected between **February 2020 and August 2020**.
- Key features include **pressure, temperature, motor current**, and other operational parameters.
- Failure reports related to **air leaks due to high stress** were used to label the data.

## **Machine Learning Models**
Three models were developed and evaluated based on accuracy, precision, recall, and F1 score:
1. **Logistic Regression:** Used as a baseline model, achieving an accuracy of **78%** but struggled with recall.
2. **XGBoost (Model A & B):** The second XGBoost model achieved an accuracy of **99.75%** and outperformed the baseline model.
3. **Neural Network Model:** Achieved an accuracy of **99.93%** based on varying architectures.

## **Feature Engineering**
- Rolling averages of **oil temperature and pressure differences** were introduced.
- **Stratified sampling** ensured that failure records were well-represented in training and testing.
- **Feature importance analysis** showed that **oil temperature, motor current, and caudal impulses** were key indicators of failure.

## **Results**
| Model | Accuracy | Precision | Recall | F1 Score |
|--------|---------|-----------|--------|---------|
| Logistic Regression | 78.37% | 42.41% | 3.32% | 70.33% |
| XGBoost Model A | 82.00% | 81.53% | 19.91% | 31.90% |
| XGBoost Model B | **99.75%** | **99.29%** | **99.36%** | **99.56%** |
| Neural Network | **99.93%** | **99.85%** | **99.90%** | **99.88%** |

## **Key Takeaways**
- **XGBoost Model B and Neural Networks** provided **highly accurate** failure predictions.
- Feature engineering played a crucial role in improving recall and precision.
- The model can be **integrated into metro maintenance systems** to enable proactive decision-making.

## **Future Enhancements**
- Deploying the model into a **real-time predictive maintenance system**.
- Exploring **deep learning models** for further improvement.
- Collecting **real-time sensor data** to validate and enhance model performance.
