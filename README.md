## Overview

Business problem: Detect malicious activity in system logs so threats are caught early on highly imbalanced data.

What this project does: Trains a PyTorch binary classifier on cyber logs (BETH dataset) to classify events as malicious vs benign.

Main result: ~0.945 test accuracy, 0.999 precision, 0.941 recall, and 0.969 F1 on a heavily imbalanced dataset.

🛡️ Cyber Threat Detection Model Using Deep Learning
Cyber threats are increasingly sophisticated, including malware 🦠, phishing 🎣, and denial-of-service attacks ⚡, posing serious risks to organizations. Traditional detection methods often fail to adapt to new attack patterns. This project uses a deep learning model to detect malicious events from system logs in the BETH dataset, classifying events as malicious (1) or benign (0) ✅.

- Actions and Methodology
A feedforward neural network was built using PyTorch 🐍 to identify cyber threats, with attention to handling class imbalance and ensuring reliable performance on rare malicious events.

- Model Design:
Fully connected neural network with three hidden layers and ReLU activations 🔧
Output layer with sigmoid activation for binary classification 🎯

- Handling Class Imbalance:
Weighted Binary Cross-Entropy Loss applied to give higher importance to rare malicious events ⚖️

- Optimization:
Adam optimizer for adaptive learning rates and faster convergence 🚀
Features scaled with StandardScaler for stable training 📊

- Evaluation:
Accuracy, precision, recall, F1 score, and confusion matrix 📈
Visualizations to confirm class imbalance and model performance 🖼️

- Observations:
High training and validation performance with accuracy around 0.99 and 0.997, indicating effective learning ✅
Testing performance: accuracy 0.945, precision 0.999, recall 0.941, F1 score 0.969 📊
Confusion matrix confirmed the model successfully identifies most malicious events while keeping false positives low ❌➡️✅
Class imbalance visualization confirmed the need for weighted loss ⚖️

- Conclusion
The model effectively detects cyber threats, demonstrating that a well-trained, relatively simple neural network can handle real-world, imbalanced datasets. Metrics and visualizations provide clear, interpretable results that can guide proactive cybersecurity measures 🛡️.
