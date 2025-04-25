

---

```markdown
# 🎬 Movie Plot Generator using distilgpt2

This project showcases how a transformer-based language model can be fine-tuned to generate unique movie plots. By using Hugging Face's `distilgpt2` and training it on a subset of the Wikipedia Movie Plot dataset from Kaggle, the model can generate creative movie storylines from just a starting prompt provided by the user.

> 🚀 The entire model is deployed in a **Streamlit app** for a user-friendly, real-time text generation experience.

---

## 📌 Table of Contents

- [Introduction](#introduction)
- [Objective](#objective)
- [Background](#background)
- [Tools & Technologies](#tools--technologies)
- [Dataset Description](#dataset-description)
- [Methodology](#methodology)
- [Training Details](#training-details)
- [Results](#results)
- [Future Work](#future-work)
- [Conclusion](#conclusion)
- [How to Run](#how-to-run)

---

## 🧠 Introduction

With the rapid advancements in natural language processing, generative models like GPT-2 are being applied in creative fields such as storytelling. This project trains a fine-tuned version of `distilgpt2` on movie plot summaries so it can generate new, original movie plots from just a sentence-long prompt.

A **Streamlit app** allows anyone to interact with the model through a web browser, making it a fun and intuitive storytelling tool.

---

## 🎯 Objective

- Fine-tune `distilgpt2` on a movie plot dataset to enhance its storytelling capabilities.
- Enable users to generate entire movie plots by providing only the beginning.
- Build a full-stack NLP system from dataset to deployment.
- Make the tool accessible to non-technical users through a Streamlit app.

---

## 🧾 Background

General-purpose language models lack narrative focus. By training `distilgpt2` on domain-specific data (movie plots), the model adapts to the language, structure, and creativity of cinematic storytelling. This makes it ideal for applications in writing assistants, idea generation, or screenplay prototyping.

---

## 🛠️ Tools & Technologies

- **Model:** distilgpt2 (`GPT2LMHeadModel`)
- **NLP Libraries:** Hugging Face `transformers`, `datasets`
- **Backend:** PyTorch
- **Data Handling:** Pandas
- **Web App:** Streamlit
- **Others:** `scikit-learn`, `tqdm`, `matplotlib`, `tokenizers`

---

## 📚 Dataset Description

The dataset used is the [Wikipedia Movie Plots Dataset (Kaggle)](https://www.kaggle.com/datasets), which includes:
- Title
- Release Year
- Director & Cast
- Genre
- Plot Summary

For training, only the **“Plot”** field was used. A subset of **1,000 plots** was selected for faster iteration and training efficiency.

---

## 🔍 Methodology

1. **Data Preprocessing:**  
   Extracted and cleaned plot summaries using Pandas.

2. **Tokenization:**  
   Used `distilgpt2` tokenizer with a max length of 128 tokens.

3. **Dataset Handling:**  
   Converted DataFrame to Hugging Face `Dataset`, then split into train/test.

4. **Model Training:**  
   Used `Trainer` API with `DataCollatorForLanguageModeling`.

5. **Generation & Inference:**  
   Applied sampling techniques (`top_k`, `top_p`) for creative outputs.

6. **Deployment:**  
   Built a **Streamlit** app that allows real-time user interaction with the model.

---

## 🏋️ Training Details

- **Epochs:** 10  
- **Learning Rate:** 2e-5  
- **Loss:** ~3.61  
- **Train/Test Split:** 80/20  
- **Global Steps:** 2740  
- **Hardware:** CPU (Local)

---

## 📈 Results

The model generates compelling and context-aware movie plots from prompts such as:

**Prompt:**  
`A short film about a pilot who`  
**Generated:**  
`is trapped in an underground submarine. The Girl At Home (1970)...`

These outputs demonstrate the model’s ability to mimic plot structure and generate logical, sometimes humorous storylines.

---

## 🔮 Future Work

- Train on the full dataset (34,000+ plots)
- Add genre-conditioning to control plot themes
- Upgrade to larger models (e.g., `gpt2-medium`, `gpt-neo`)
- Collect user feedback in-app for reinforcement learning
- Deploy on Hugging Face Spaces or cloud servers

---

## ✅ Conclusion

This project proves that even beginner-friendly models like `distilgpt2` can be fine-tuned to generate creative text outputs. Combined with a web-based UI using Streamlit, it offers an engaging and accessible tool for both developers and storytellers alike.

---



### 📩 Contact

For questions or suggestions, feel free to open an issue or connect on [LinkedIn](https://www.linkedin.com/in/subham-das-3b2624147).

```

---
