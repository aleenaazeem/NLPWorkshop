# NLP Similarity Model Evaluation

This repository contains code to evaluate different NLP models for word similarity tasks using the **WordSim-353** dataset. The goal is to find the best-performing model based on the **Spearman correlation** score.

## 📌 Project Overview
- Uses **SentenceTransformer** models to compute similarity between word pairs.
- Evaluates performance using **Spearman correlation** with human-labeled scores.
- Compares multiple pre-trained models to determine the best one.

## 🚀 How to Use
1. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
2. **Run the notebook**: Execute the Jupyter Notebook to test different models and obtain their Spearman scores.
3. **Replace model names**: Modify the model name in the code to experiment with different SentenceTransformer models.

## 📊 Results
| Model Name | Spearman Score |
|------------|---------------|
| multi-qa-mpnet-base-cos-v1 | 0.787 ✅ (Best so far) |
| paraphrase-mpnet-base-v2 | 0.7748 |
| paraphrase-MiniLM-L6-v2 | 0.7727 |

## 📌 Best Model for Q&A Tasks
If you're working on **Q&A retrieval**, try:
- **"multi-qa-mpnet-base-dot-v1"** ✅ Best for general Q&A
- **"multi-qa-mpnet-base-cos-v1"** (used in this project)
- **"multi-qa-distilbert-cos-v1"** (faster but slightly less accurate)

## 📬 Contact
For any questions, feel free to reach out or contribute to the project!

---
📌 **Future Work**: Exploring fine-tuning to further improve performance. 🚀

