# 🧠 Fine-Tuning Product Titles with Descriptions using Ollama

This repository contains a series of Jupyter notebooks for fine-tuning a language model (via **Ollama**) to generate **product titles from descriptions** — and vice versa. The goal is to experiment with different input/output combinations and evaluate the effectiveness of fine-tuning.

## 🔧 Notebooks Overview

### `1. Prepare_Dataset.ipynb`
This notebook processes the original `trn.json` dataset by adding `title` and `description` fields.

- **Input**: `description`  
- **Output**: `title`  
- Purpose: To train the model to generate accurate product titles based on a detailed description.

---

### `2. Fine_Tuning_with_Dataset.ipynb`
Performs **fine-tuning** using the dataset prepared in step 1, leveraging the **Ollama model**.

- Includes detailed comments to explain each step.
- Contains examples of successful inference — e.g., given a description from the test dataset, the model correctly returned the corresponding product title.

---

### `3. Prepare_Dataset (In: Title, Out: Desc - optional).ipynb`
An optional notebook to reverse the direction:

- **Input**: `title`  
- **Output**: `description`  
- Purpose: Shows that the model can also be trained to generate descriptions from titles.

---

### `4. Test_without_FineTuning.ipynb`
Tests the model **without fine-tuning**:

- Given a product description, the base model completes the sentence generically.
- It does **not** return the expected product name, highlighting the impact of fine-tuning.

---

## 🧠 Model
- **Model Used**: [Ollama](https://ollama.com) – a lightweight and local-friendly solution for running and fine-tuning LLMs.

---

## 🚀 Why This Matters
- Automates product catalog generation.
- Demonstrates the practical benefits of small-scale fine-tuning.
- Enables both directions: description → title and title → description.

---

Feel free to fork, explore, and adapt these notebooks for your use case. Contributions welcome!
