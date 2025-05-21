
# 📰 BBC News Summarizer using T5

This project demonstrates how to fine-tune the T5 transformer model on a real-world dataset to generate concise, abstractive summaries of BBC news articles. It showcases an end-to-end NLP pipeline — from preprocessing to model evaluation — implemented entirely in a single Jupyter notebook.

---

## 📁 Dataset

**BBC News Summary Dataset**  
Source: [Kaggle](https://www.kaggle.com/datasets/pariza/bbc-news-summary)

- Contains two folders: `News Articles/` and `Summaries/`
- Articles and summaries are organized into 5 categories: `Business`, `Politics`, `Sports`, `Tech`, and `Entertainment`
- Each article has a corresponding summary with matching filenames

---

## 📌 Project Highlights

- 🧠 Fine-tuning of Hugging Face’s `T5-small` for text summarization
- 🔍 Data analysis: article and summary lengths, class distribution, data integrity
- 🧹 Preprocessing with `spaCy` (lowercasing, punctuation removal, whitespace cleanup)
- 📊 Evaluation using ROUGE metrics
- 🧪 Test interface: provide a news article and generate a summary

---

## 🚀 Getting Started

You can run the entire project in a **Kaggle Notebook** or locally in a Jupyter environment.

### ✅ Requirements (Kaggle Kernels Already Have These)

- Python ≥ 3.7  
- Hugging Face Transformers  
- Hugging Face Datasets  
- spaCy  
- Matplotlib  
- Scikit-learn

To install dependencies locally:

```bash
pip install transformers datasets spacy scikit-learn matplotlib
python -m spacy download en_core_web_sm
```

---

## ▶️ Running the Project

1. Clone this repository or open the notebook directly on Kaggle.
2. Download the dataset from [Kaggle](https://www.kaggle.com/datasets/pariza/bbc-news-summary) and place it in the appropriate directory.
3. Run the notebook cell by cell to:
   - Analyze the dataset
   - Preprocess text
   - Tokenize and prepare for training
   - Fine-tune the T5 model
   - Evaluate using ROUGE
   - Test the summarizer with your own article

---

## 📈 Results

After 30 epochs of training:

- **ROUGE-1**: ~0.23  
- **ROUGE-2**: ~0.19  
- **ROUGE-L**: ~0.22  

The model performs reasonably well on short-form summarization for the five BBC news categories.

---

## 🏁 Conclusion

This project demonstrates how transformer-based models can be adapted for abstractive summarization using modest-sized datasets. With clean preprocessing and task-specific fine-tuning, T5 can generate coherent and readable summaries that align closely with human-written ones.

For future improvements:
- Experiment with `T5-base` or `BART`
- Add length control to prevent repetition or truncation
- Use beam search or top-k sampling in generation

---

## 📌 Author

**Syed Abdullah Hasan**  
Aspiring AI Engineer | NLP & Computer Vision Enthusiast
