
# Multi-Task & Emotion Analysis    (don't give a fck, it's shit (used ai))

This project builds a **multi-task learning** model to classify text for three tasks:
1. **Aspect-Based Sentiment Analysis** (positive/negative/neutral) 💡
2. **Emotion Detection** (happy/sad/angry) 😄😢😡
3. **Sentiment-Emotion Joint Modeling** (combining sentiment & emotion) 

## 📋 Requirements
- Python 3.6+
- TensorFlow (Keras) & PyTorch
- Libraries: pandas, numpy, nltk, spacy, scikit-learn, etc.

Install all dependencies with:
```bash
pip install -r requirements.txt
```

## 🚀 Setup & Installation
1. Clone the repo:
   ```bash
   https://github.com/JeetChaurasia/Multi-Task-Learning-MTL-Model.git
   ```
2. Download the spaCy model:
   ```bash
   python -m spacy download en_core_web_sm
   ```
3. Get the **Semeval-2014 dataset** and save as `semeval2014_train.csv` & `semeval2014_test.csv`.

## 🧠 Model Architecture
- **Input**: Preprocessed text (tokenized, stopword removed)
- **Embedding Layer**: Converts tokens to dense vectors
- **LSTM Layer**: Captures text sequence dependencies
- **Outputs**:
  - Aspect Sentiment (positive/negative/neutral)
  - Emotion (happy/sad/angry)

Adversarial training improves model robustness using **PyTorch**.

## 🎓 Training
Train the model with:
```bash
python train.py
```

### ⚡ Metrics:
- **Accuracy** 📊
- **F1 Score** 🔥
- **ROC AUC** 🎯
- **MSE** 📉

## 📝 Save/Load Model
Save the model with:
```python
model.save('multi_task_learning_model.h5')
```
Load the model:
```python
loaded_model = keras.models.load_model('multi_task_learning_model.h5')
```

## 📄 License
MIT License - see [LICENSE](LICENSE) for details.

```




