#  IoT Intrusion Detection Using Machine Learning & Deep Learning  

##  Project Overview  
This project focuses on **intrusion detection in IoT devices** using **machine learning and deep learning models**. With the increasing number of IoT devices, cybersecurity threats are becoming more sophisticated. This study aims to build an efficient **Intrusion Detection System (IDS)** that can classify various types of network attacks using the **CICIOT2023 dataset**.  

##  Models Used  
We implemented and compared the following models:  

### ** Deep Learning Models**  
- **LSTM (Long Short-Term Memory)** – Best for sequential data (Achieved **99.89% accuracy**).  
- **GRU (Gated Recurrent Unit)** – Similar to LSTM but computationally more efficient (**98.69% accuracy**).  
- **Deep CNN (Convolutional Neural Network)** – Extracts spatial patterns from network traffic (**98.34% accuracy**).  

### ** Machine Learning Models**  
- **Decision Tree** – Simple yet effective rule-based classification (**99.37% accuracy**).  
- **XGBoost (Extreme Gradient Boosting)** – Fast and accurate boosting algorithm (**99.30% accuracy**).  

##  Dataset  
We used the **CICIOT2023 dataset**, which consists of:  
- **105 IoT devices** (Smart home, Zigbee, Z-Wave, etc.)  
- **33 different attack types** (DDoS, DoS, Brute Force, Mirai, etc.)  
- **47 features** extracted from network traffic logs.  

##  Preprocessing Steps  
- **Handling Missing Values**  
- **Feature Selection Using Correlation Analysis**  
- **Label Encoding for Categorical Features**  
- **Standardization Using StandardScaler**  
- **Splitting Dataset (70% Train, 30% Test)**  

##  Model Training & Evaluation  
Each model was trained and evaluated using the following metrics:  
 **Accuracy**  
 **Precision, Recall, F1-score**  
 **False Positive Rate (FPR)**   

| Model       | Accuracy  | Precision | Recall | F1-score |
|------------|----------|-----------|--------|----------|
| **LSTM**        | **99.89%**   | 99.72%    | 99.85% | 99.78%   |
| **GRU**         | 98.69%   | 98.41%    | 98.54% | 98.47%   | 
| **Deep CNN**    | 98.34%   | 98.58%    | 97.00% | 97.20%   | 
| **Decision Tree** | 99.37%  | 99.00%    | 99.10% | 99.05%   | 
| **XGBoost**     | 99.30%   | 0.85 (macro avg) | 0.73 (macro avg) | 0.75 (macro avg) | 

##  Key Findings  
**LSTM performed best**, achieving **99.89% accuracy**, but required longer training time.  
**GRU and CNN models also showed strong performance** with high accuracy and stability.  
**Decision Trees & XGBoost were faster** and still highly accurate, making them suitable for real-time detection.  
**Class imbalance affected recall for rare attack types** (e.g., Backdoor Malware, Uploading Attack).  

