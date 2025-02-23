# **Pregnancy Health Risk Prediction**

## **Project Scope and Overview**

Pregnancy-related health complications pose significant risks to both mothers and babies, making early prediction crucial for effective medical intervention. This project leverages machine learning to assess pregnancy health risks based on demographic, medical, and lifestyle factors. By evaluating various machine learning algorithms, the goal is to identify the most accurate model for predicting potential health complications, ultimately aiding in better prenatal care and decision-making.

## **Dataset**

I got my dataset from [kaggle](https://www.kaggle.com/datasets/csafrit2/maternal-health-risk-data) and it was collected from different hospitals, community clinics, maternal health cares through the IoT based risk monitoring system. It includes features such as:

- **Age:** Age in years when a woman is pregnant.
- **SystolicBP:** Upper value of Blood Pressure in mmHg, another significant attribute during pregnancy.
- **DiastolicBP:** Lower value of Blood Pressure in mmHg, another significant attribute during pregnancy.
- **BS:** Blood glucose levels is in terms of a molar concentration, mmol/L.
- **HeartRate:** A normal resting heart rate in beats per minute.
- **Risk Level:** Predicted Risk Intensity Level during pregnancy considering the previous attribute.

# Risk Classes
- **Low Risk (0)**
- **Medium Risk (1)**
- **High Risk (2)**


### **Model Performance Table**

| Model | Optimizer | Regularization | Epochs | Early Stopping | Layers | Learning Rate | Accuracy | F1 Score | Recall | Precision | AUC |
|--------|------------|---------------|--------|---------------|--------|--------------|----------|----------|--------|-----------|------|
| **Instance 1** | - | - | 100 | No | 2 | 0.001 | 65.00% | 0.66 | 0.67 | 0.67 | 0.64 |
| **Instance 2** | Adam | L1 | 100 | Yes | 2 | 0.001 | 64% | 0.62 | 0.65 | 0.62 | 0.64 |
| **Instance 3** | Adam | L2 | 100 | Yes | 2 | 0.001 | 61% | 0.58 | 0.62 | 0.59 | 0.61 |
| **Instance 4** | RMSprop | L1_L2 | 100 | Yes | 2 | 0.0001 | 63% | 0.61 | 0.64 | 0.62 | 0.633 |
| **Instance 5**  | RMSprop | L2 | 100 | Yes | 2 | 0.001 | 61% | 0.59 | 0.62 | 0.59 | 0.61 |
| **Random Forest Model** | - | - | - | - | - | - | 77% | 0.78 | 0.78 | 0.78 | 0.77 |

---

## **Best Model**
The best model was the Random forest model with an Accuracy of 77% which was higher than that of all the Neural Networks.

---


## **Video**

[**Watch Here**](https://www.youtube.com/watch?v=SnD2CkG9AoE)

---

## **Conclusion**
This project demonstrates the potential of machine learning in predicting pregnancy-related health risks, offering a data-driven approach to improving maternal care. By analyzing key demographic, medical, and lifestyle factors, the models provide valuable insights that can assist healthcare professionals in early risk detection and intervention. While the results are promising, further work is needed to enhance model accuracy, incorporate larger datasets, and refine predictive features. Future developments could include integrating real-time data sources and expanding accessibility to support broader healthcare applications.


