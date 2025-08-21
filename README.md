## 🔬 Privacy-Preserving Pneumonia Detection from Chest X-rays  

> 📄 **Accepted at IC3 Conference 2025** 🎉  
> Research on **AI-driven pneumonia detection** while ensuring **patient data privacy**.  

---

### 📌 Overview  
This work provides a **comparative analysis of privacy-preserving techniques** applied to **chest X-ray pneumonia detection**.  
We explored:  
- 🧩 **Federated Learning (FL)**  
- 🔒 **Differential Privacy (DP – Gaussian & Laplace)**  
- 🖼️ **Pixelation**  
- ⚡ **Hybrid FL + DP approaches**  

Our goal was to study the **privacy–utility trade-off**, ensuring compliance with **healthcare privacy laws (HIPAA)** while maintaining **diagnostic accuracy**.  

---

### 🔑 Key Insights  
✔️ **Federated Learning** delivered the highest accuracy (**85.90%**) using decentralized training  
✔️ **Gaussian DP** achieved the best privacy–utility balance (**83.17% accuracy, 94.10% recall**)  
✔️ Optimal **privacy budget range:** `ε ∈ [2.0, 4.0]`  
⚠️ Hybrid models (**FL + DP**) introduced too much complexity, reducing performance  

---

### 📊 Results  

#### 🏥 Model Performance Comparison
| Method              | Test Accuracy (%) | Precision (%) | Recall (%) | F1 Score (%) |
|---------------------|------------------:|--------------:|-----------:|-------------:|
| Baseline CNN        | 81.89             | 78.55         | **97.69**  | 87.08        |
| **Federated Learning**  | **85.90**         | **88.16**     | 85.90      | 85.05        |
| **Gaussian DP**     | 83.17             | 81.74         | 94.10      | **87.49**    |
| Laplace DP          | 62.02             | 62.77         | 96.41      | 76.03        |
| Pixelation          | 57.15             | 52.00         | 87.46      | 65.20        |
| FL + DP Hybrid      | 37.50             | 18.75         | 50.00      | 27.27        |

---

#### 📂 Dataset Distribution
| Category   | Training | Validation | Test | Total |
|------------|---------:|-----------:|-----:|------:|
| Normal     | 1,341    | 8          | 234  | 1,721 |
| Pneumonia  | 3,875    | 8          | 390  | 4,135 |
| **Total**  | **5,216**| **16**     | **624** | **5,856** |

---

#### 🔐 Privacy Budget Analysis (DP)
| Privacy Budget (ε) | Gaussian DP Accuracy (%) | Laplace DP Accuracy (%) |
|--------------------|-------------------------:|------------------------:|
| 0.1                | 52.3                    | 45.1                   |
| 0.5                | 67.8                    | 58.2                   |
| 1.0                | 75.4                    | 62.0                   |
| 2.0                | 81.2                    | 64.5                   |
| 4.0                | **83.1**                | 65.8                   |
| 8.0                | 83.2                    | 66.0                   |
| 10.0               | 83.2                    | 66.1                   |

---

### 🏆 Contribution to Research  
This work offers:  
- Practical guidelines for **designing privacy-preserving medical AI systems**  
- Benchmarking results to balance **accuracy vs. privacy**  
- Insights into **real-world deployment under HIPAA compliance**  

---

✨ *This project combines the fields of **Healthcare AI, Federated Learning, and Differential Privacy**, aiming to make diagnostic systems both **powerful and trustworthy.***
