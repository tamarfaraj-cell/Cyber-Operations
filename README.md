Overview
This project implements a high-fidelity, hybrid Anomaly-Based Intrusion Detection System designed for diverse network environments including Robotics (ROS), Autonomous Vehicles (UAVs), Enterprise IT, and Modern IoT. The system utilizes a multi-model comparison suite to identify the most effective machine learning algorithms for detecting contemporary cyber threats.

Key Features
1. Multi-Dataset Support: Analysis performed on ROSIDS23, UAVAttack, CICIDS2017, and CICIIoT2025 datasets.
2. Advanced Data Balancing: Integration of SMOTE (Synthetic Minority Over-sampling Technique) to handle class imbalances between benign and malicious traffic.
3. Performance Optimization: Implementation of Stochastic Gradient Descent (SGD) for fast SVM training and Subsampling for efficient large-scale data processing.
4. Academic Validation: Use of 10-Fold Cross-Validation to ensure model robustness and generalization.
5. Visualization Suite: Generation of Precision-Recall (PR) curves, Side-by-Side Confusion Matrices, and Accuracy comparisons.

Models Evaluated
The research script compares the following five algorithms:

1. Random Forest: (configured with 30-50 estimators for speed/accuracy balance).
2. Decision Tree: (standard CART implementation).
3. Logistic Regression: (optimized with 500-1000 iterations).
4. Fast SVM (SGD): (utilizing modified Huber loss for probabilistic output).
5. K-Nearest Neighbors (KNN): (optimized with parallel processing using all CPU cores).


Project Structure
1. advanced_research.py: The master script containing the 10-fold CV and 5-model comparison suite.
2. IoT_2025_Analysis.py: Specific analysis script for modern IoT threat detection.
3. UAV_Analysis.py: Specialized script for UAVCAN protocol anomaly detection.
4. ROS_Robotics_Analysis.py: Script focused on Robot Operating System (ROS) node security.
5. datasets/: Directory containing CSV files for the respective environments.

