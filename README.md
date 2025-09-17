## Web Security Analysis and Cyber Attack Detection
# Introduction
In an increasingly digital world, web applications are a cornerstone of modern interaction, but this reliance has made them vulnerable to various security threats. This repository presents an analysis of a dataset containing records of four major cyber attack types: 

XSS (Cross-Site Scripting), DDoS (Distributed Denial-of-Service), CSRF (Cross-Site Request Forgery), and SQL Injection (SQLi). These attacks target web applications, servers, and users to steal data, disrupt services, or exploit vulnerabilities.


## Major Cyber Attacks
The project analyzes the following types of cyber attacks:


XSS Attack: An attacker injects malicious scripts (JavaScript) into web pages. When a user visits the compromised page, the script runs in their browser, allowing attackers to steal session cookies, credentials, or sensitive data, and even deface websites or redirect users to malicious sites.




CSRF Attack: This attack tricks an authenticated user into performing unintended actions on a trusted website by exploiting the user's active session. This can be used to change account settings, such as a password or email, or perform unauthorized transactions.



DDoS Attack: Attackers overload a server, website, or network with excessive traffic, making it slow or completely unavailable to legitimate users. A network of infected devices, known as a botnet, is often used to flood the target with requests. Consequences include website downtime, increased server costs, and potential security risks used to distract security teams while another attack occurs.





SQL Injection: An attacker injects malicious SQL queries into a web application's input fields to manipulate the database. This can allow attackers to steal sensitive data (usernames, passwords, financial records), modify or delete database records, or bypass authentication to gain unauthorized access.


## Dataset Overview
The dataset used for this analysis contains 20,000 records related to web security attacks across 11 columns, including details about application names, permissions, API usage, websites, IP addresses, request types, and attack classifications.

## Key Highlights:


Total Attacks Identified: 15,892 


Non-Attack Requests: 4,108 


# Attack Distribution: The dataset provides valuable insights into the most common web security threats.


DDoS: 4,053 cases 


XSS: 3,957 cases 


SQL Injection: 3,949 cases 


CSRF: 3,933 cases 

## Data Preprocessing
The following steps were taken to prepare the data for analysis:


Handling Missing Values: Missing values in the "Location" and "Attack Type" columns were handled using forward-filling.


Label Encoding: LabelEncoder() was used for multiple categorical features.


Splitting Data: The dataset was split into training and testing sets using train_test_split(X, y, test_size=0.10, random_state=10).


Feature Scaling: StandardScaler() was used to scale numerical features.

Model Building
Various machine learning models were built to detect cyber attacks. The project used the following libraries and models:

## Python Libraries:


pandas for data handling and manipulation 


numpy for numerical operations 


matplotlib.pyplot and seaborn for data visualization 


sklearn for data preprocessing, model selection, and evaluation 



xgboost for the XGBoost model 


joblib to save and load trained models 

Machine Learning Models:

Logistic Regression 

Decision Tree Classifier 

Random Forest Classifier 

Support Vector Machine (SVC) 

K-Nearest Neighbors (KNeighborsClassifier) 

XGBoost Model (XGBClassifier) 

## Key Prevention Strategies
Proactive security measures are crucial to mitigate risks and ensure safer digital interactions. Key strategies include:


Network Security: Use firewalls, intrusion detection/prevention systems (IDS/IPS), and VPNs.

Application Security: Practice secure coding, input validation, and use web application firewalls (WAFs).

Data Security: Implement encryption, access controls, and secure backups.

User Security: Enforce multi-factor authentication (MFA), strong password policies, and user education.

Threat Monitoring: Conduct continuous security audits, penetration testing, and real-time anomaly detection.

## Conclusion
The analysis highlights the significant threats posed by cyberattacks like XSS, DDoS, CSRF, and SQL Injection. APIs like 

getCellLocation, sendTextMessage, and getSubscriberId are frequently targeted, emphasizing the need for stricter security controls. Regular vulnerability assessments and secure coding practices are essential as web applications continue to evolve.
