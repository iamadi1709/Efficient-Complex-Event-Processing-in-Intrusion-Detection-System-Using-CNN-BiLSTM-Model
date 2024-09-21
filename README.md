**🚀 Efficient Complex Event Processing in Intrusion Detection System Using CNN-BiLSTM Model 🌐**

![image](https://github.com/user-attachments/assets/4fb4854a-82d1-47b7-a5c9-34314ab6046a)

Intrusion Detection Systems (IDSs) are the digital guardians 🛡️ of our computer networks, defending them from malicious attacks. This project presents a hybrid CNN-BiLSTM model for real-time intrusion detection using Complex Event Processing (CEP). Unlike traditional IDS, which struggles with new and unidentified threats, our system detects both known and unknown attacks, just like a skilled detective 🕵️‍♂️ piecing together clues from network traffic.

![image](https://github.com/user-attachments/assets/6f5fe057-c251-45bd-b0a7-279c3f836ebe)

📑 **Abstract: Intrusion detection systems are essential for securing computer networks against cyberattacks. However, conventional IDSs fail to detect unusual or unknown attacks as they rely on the signature of known threats. This project introduces a CNN-BiLSTM hybrid model that leverages Complex Event Processing (CEP) for real-time attack detection. Using the CIC-IDS2017 dataset, our model can successfully identify multiple attack categories that traditional methods often miss. I have compared the performance of this model against Random Forest, which showed higher accuracy but the CNN-BiLSTM demonstrated significant promise in handling unknown threats.**

![image](https://github.com/user-attachments/assets/a63f69b9-be88-4e81-9b8f-98ff452a2591)

**🔍 Dataset Overview**
**CIC-IDS2017 Dataset:**

**Entries: 2.8+ million packets**
**Duration: Captured over 7 days**
**Attack Scenarios: Brute Force, Heartbleed, Botnet, DoS, DDoS, Web Attack, Infiltration**
**Classes: Highly imbalanced with most records in the 'Benign' class**
**Features: 78 numerical features + 1 label column.**

**🛠️ Project Steps**
**1. Load and Analyze Data 📊**
Analyze rows, columns, and dataset structure

**2. Data Cleaning 🧼**
Handle missing values, duplicates, and outliers

**3. Exploratory Data Analysis 🔍**

Visualizations, correlation matrix, and feature pattern analysis

**4.Data Preprocessing 🛠️**
Remove duplicates, handle missing values, downcast data types

**5.Dimensionality Reduction 🔻**
Apply PCA to reduce high-dimensional data

**6. Model Training 🤖**
Train with Random Forest, Logistic Regression, SVM, Decision Tree, KNN

**7. Performance Evaluation 📈**
Evaluate using Accuracy, Recall, F1-score, Confusion Matrix

![image](https://github.com/user-attachments/assets/c3d5d689-ad4d-41ef-8146-2fd1e8365ff9)

**🔍 Exploratory Data Analysis**
We discovered:

Duplicates: 308,381 rows (removed for unbiased results)
Missing Data: 0.06% of the data contained missing or infinite values, handled accordingly
Correlations: Detected multicollinearity between several features

**⚙️ Data Preprocessing**
Duplicates: Removed 308,381 duplicate rows
Missing Values: Replaced missing and infinite values with the median
Downcasting: Reduced memory usage by downcasting data types
PCA: Reduced dimensionality while preserving data integrity using Incremental PCA

**🔥 Machine Learning Models**
We implemented various models to tackle both Binary Classification (normal vs. anomalous traffic) and Multi-Class Classification (identifying specific attack types):

Logistic Regression
Support Vector Machine (SVM)
Random Forest Classifier
Decision Tree
K-Nearest Neighbours (KNN)
Our Random Forest model emerged as a top performer, excelling in both binary and multi-class classification.

**🔄 Hybrid CNN-BiLSTM Model**
The CNN-BiLSTM hybrid model was employed for handling sequential network traffic data. It captures both the spatial and temporal features of network packets, detecting patterns that can signal unknown attacks.

**🔬 Comparison with Random Forest:** Random Forest achieved slightly better accuracy, but the CNN-BiLSTM model showed promising results, especially for **previously unseen attack patterns.**

**🚀 Performance Evaluation**
We evaluated all models using:

Accuracy
Recall
F1-Score
Confusion Matrix

<img width="829" alt="image" src="https://github.com/user-attachments/assets/3685dd97-f4e6-4ec5-9378-7314f539945a">

**Model	                  Accuracy	         Recall	           F1-Score**
**Random Forest	           98.5%	           97.3%	            97.8%**

**CNN-BiLSTM	             97.2%	           96.1%	            96.5%**

**Support Vector Machine	94.6%	             92.3%	            93.0%**

**📊 Visualizations**
Here are some key visualizations used in our analysis:

📈 Correlation Heatmap: Identifying multicollinearity
📊 Attack Distribution: Imbalance of benign vs attack traffic
📉 PCA Components: Visualizing dimensionality reduction

**🚀 Future Work**
🔄 The prospective investigation on this matter can involve utilising the intrusion detection system (IDS) on a bigger and more complex network. The system may be substantially improved to detect both tried intrusions and also attacks that already occurred. Alteration of classification algorithms would spend less time doing analysis, it will therefore be able to catch cases at a much higher rate. Shortening the time of detection and making detecting the process more accurate will be performed with the help of better algorithms. In addition, future work should deal with expanding the range of threats addressed especially inside complex networks in order to let the IDS operate optimally.

**👨‍💻 Author**
Aditya Kumar Singh
LinkedIn: https://www.linkedin.com/in/iamadi1709/

Email: adityakumar.singh2020a@vitstudent.ac.in

⭐️ Show Your Support
If you found this project interesting or useful, feel free to give it a ⭐️ on GitHub! 😄

Thanks & Regards
Aditya Kumar Singh
