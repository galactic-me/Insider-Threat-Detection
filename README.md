# Insider-Threat-Detection
Insider Threats are a form of cybersecurity challenges that are caused by insider employees/working officials inside an organization.  Why is it a challenge? Surveys tell that around 90% of the cybersecurity challenges are due to insider threats so they need to be tackled. Insiders posess unauthorized access and information that they may exploit.
AVAILABLE DATA:
Based on the available data, we have approaches varied for different types of data:
1)Sequential Data: This includes the time-series data.It uses both ML and DL techniques.
2)Non-Sequential Data: It comprises of the image data to identify insider threats. They are possible using Neural Networks.

Data Collection: 
Data is collected from CMU CERTv4.2 Dataset (for WCNN). CERTv 5.2 dataset is used for Machine Learning Algorithms.
Data is stored in unified formats. The two main sources are user activities , organization structure and user profile information.

Data Preprocessing: 
It involves aggregation of data from various log files into a single user file. The dataset contains multiple csv files. This if followed by feature extraction and feature selection. Frequency based and statistical features are retrieved from the user logs to improve threat detection.
We perform data processing in steps to obtain three levels of data granularity namely user-session, user-week and user-day.

Frequency features : Number of emails sent, number of long on after hour, number of USB connects to PC.
Statistical Features: Email size, file size, number of words in website visit.

Imbalance Handling: An imbalanced Dataset is one having uneven distribution of quantity of samples within distinct classifications. One class has significantly more instances than another. Due to this, model tends to perform poorly on the minority class because it tends to be biased towards the majority class.
For handling imbalances in the dataset, we use algorithms such as SMOTEENN(Synthetic Minority Over Sampling Technique and Edited Nearest Neighbours). SMOTE is for oversampling the minority classes(it increases the number of samples) ad ENN is used to remove miss-classified instances from all the classes.

Performance Metrics:
Here, the performance is measured based on ROC-AUC Curve. ROC(Receiving Characteristic Curve) depicts the relationship rate between detection rate and false positive rate under different decision thresholds .

RESULTS:
Autoencoders exhibit the best performance in detecting anomalies representing insider threats, especially at very low FPRs. LOF performs well on lower data counts.
BEST DATA REPRESENTATION: PERCENTILE REPRESENTATION. COFIRMED BY FRIEDMAN TEST.
