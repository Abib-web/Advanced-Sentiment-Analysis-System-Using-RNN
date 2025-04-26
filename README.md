# 🎬 Advanced Sentiment Analysis with RNNs – IMDb Reviews

## 📌 Project Overview and Objectives

This project is part of the course **GEI1092 – Techniques d’intelligence artificielle**.  
Our objective was to design and implement a deep learning-based **sentiment analysis system** using **Bidirectional LSTM (RNNs)** on the **IMDb movie review dataset**.

The model classifies reviews as **positive** or **negative**, and integrates several advanced tools:

- Data preprocessing pipeline  
- Sequence vectorization  
- Deep learning model with Bidirectional LSTM  
- Model evaluation and explainability with **SHAP** and **LIME**  
- Carbon emission tracking using **CodeCarbon**  
- Deployment on embedded systems via **TensorFlow Lite**

---

## 📂 Dataset Download and Preprocessing

You can download the IMDb dataset here:  
📎 https://ai.stanford.edu/~amaas/data/sentiment/

### 🧹 Preprocessing Steps

- Convert text to lowercase  
- Remove HTML tags and punctuation  
- Remove stopwords using NLTK  
- Tokenize using Keras `Tokenizer`  
- Convert text to padded integer sequences of length **200**

> Scripts and code are available in the notebook: `Mini_Project_2.ipynb`

---

## 🧠 Model Training and Evaluation

The model architecture includes:

- Two **Bidirectional LSTM** layers  
- Dropout and Dense layers  
- `binary_crossentropy` loss function  
- `Adam` optimizer  
- `EarlyStopping` for better generalization

### ✅ Performance:

- Accuracy: **~85%** on test data  
- Confusion matrix and manual sentence testing included  
- Sample reviews are tested to validate real-world behavior

---

## ♻️ Carbon Footprint Analysis

We used the **CodeCarbon** library to monitor the **energy usage** and **CO₂ emissions** during training.  
Although our project remains lightweight, this step raises awareness about the **environmental impact of AI models**.

---

## 🔍 Ethical Considerations and Explainability

To ensure the **fairness** and **transparency** of our model:

- We used **SHAP** and **LIME** to understand how the model makes predictions.  
- These tools helped visualize which words influenced the classification.  
- We identified that ambiguous phrases lead to uncertain predictions, which we highlighted in our evaluation.  
- We also reflected on the **risk of biases** in training data and the importance of careful dataset curation.

---

## 📱 Embedded Deployment (TensorFlow Lite)

The trained Keras model was converted to **TensorFlow Lite** to enable inference on mobile or embedded devices.

### ⚙️ Deployment Details:

- Model size (TFLite): **6.5 MB**  
- Inference time per sample: **~0.027 s**  
- Accuracy retained after conversion: **~84.9%**

This allows real-time predictions on resource-limited environments like **Raspberry Pi** or **microcontrollers**.

---

## 🧾 License and Code Release Responsibility

This project is released under the **MIT License**, which allows reuse and modification with attribution.  
We encourage open collaboration and welcome issues and pull requests.

### ✅ Responsibilities:

- Maintain transparency of model structure and training process  
- Document preprocessing steps clearly  
- Ensure ethical use of the system in real-world contexts

---

## 🛠️ Bug Reporting and Contributions

- Use the **Issues** tab to report bugs or suggest improvements  
- Open a **Pull Request** for code contributions or documentation updates  
- All code and experiments are documented in the notebook

---

## 👥 Contributors

- **Oumar Kone**  
- **Abdoul Nasser Adamou**  
- Supervisor: **Prof. Ahmed Messaoud**  
  Université du Québec à Trois-Rivières
