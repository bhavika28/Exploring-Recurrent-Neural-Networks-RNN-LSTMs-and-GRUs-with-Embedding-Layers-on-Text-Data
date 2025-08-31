# 🧠 Exploring Recurrent Neural Networks (RNN, LSTM & GRU) with Embedding Layers on Text Data

🎯 **Business Problem**  
Sequential text data requires models that can capture temporal dependencies and semantic meaning. This project explores the effectiveness of **RNNs, LSTMs, and GRUs** with **embedding layers** for text classification, comparing different architectures to identify the most accurate and efficient model.

---

## 📊 Dataset & Approach
- **Input**: Text dataset (pre-tokenized into sequences of words).  
- **Vocabulary Size**: Top 10,000 most frequent words retained.  
- **Representation**: Each word is mapped to an integer index → converted into embedding vectors.  
- **Splits**: Training, validation, and test sets.  

---

## 🔑 Key Experiments

### **Task 1: Vanilla RNN**
1. **RNN with Sigmoid Activation**  
   - Hidden dimension = 64  
   - Output: Sigmoid neuron  

2. **RNN with Global MaxPooling + ReLU**  
   - Hidden dimension = 64  
   - Global MaxPooling1D → Dense(16, ReLU) → Dense(1, Sigmoid)  

---

### **Task 2: LSTM**
1. **LSTM with Sigmoid Activation**  
   - Hidden dimension = 64  
   - Output: Sigmoid neuron  

2. **LSTM with Global MaxPooling + ReLU**  
   - Hidden dimension = 64  
   - Global MaxPooling1D → Dense(16, ReLU) → Dense(1, Sigmoid)  

3. **Stacked LSTMs with Global MaxPooling + ReLU**  
   - Two stacked LSTM layers (hidden dimension = 64 each)  
   - Global MaxPooling1D → Dense(16, ReLU) → Dense(1, Sigmoid)  

---

### **Task 3: GRU**
1. **GRU with Sigmoid Activation**  
   - Hidden dimension = 64  
   - Output: Sigmoid neuron  

2. **GRU with Global MaxPooling + ReLU**  
   - Hidden dimension = 64  
   - Global MaxPooling1D → Dense(16, ReLU) → Dense(1, Sigmoid)  

---

## 📈 Performance Evaluation
Each model was trained and evaluated on:  
- ✅ Test Accuracy  
- 📉 Training Loss vs Validation Loss  
- 📊 Training Accuracy vs Validation Accuracy  

---

## 📊 Results Comparison

| Model Variant                        | Test Accuracy | Notes |
|--------------------------------------|---------------|-------|
| Vanilla RNN (Sigmoid)                | ~XX%          | Baseline sequence model |
| RNN + Global MaxPooling + ReLU       | ~XX%          | Improved generalization |
| LSTM (Sigmoid)                       | ~XX%          | Better long-term memory |
| LSTM + Global MaxPooling + ReLU      | ~XX%          | Balanced performance |
| Stacked LSTM + Pooling + ReLU        | ~XX%          | Highest accuracy |
| GRU (Sigmoid)                        | ~XX%          | Efficient alternative |
| GRU + Global MaxPooling + ReLU       | ~XX%          | Tradeoff: accuracy vs speed |

*(Replace `XX%` with actual results after training.)*

---

## 🛠️ Technologies Used
- Python  
- TensorFlow / Keras (or PyTorch, depending on implementation)  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Jupyter Notebook  

---

## 🚀 Quick Start

### Prerequisites
Install dependencies:
```bash
pip install tensorflow pandas numpy matplotlib seaborn jupyter
```

Clone the repository
```bash
git clone https://github.com/your-username/rnn-text-classification.git
cd rnn-text-classification
```

Run the notebooks
```bash
jupyter notebook RNN_LSTM_GRU_Text.ipynb
```

## 🔬 Technical Highlights

- Embedding Layer: Word indices mapped to dense vectors of size 64.
- Model Architectures: Vanilla RNN, LSTM, GRU with pooling and stacked variations.
- Performance Evaluation: Training/validation accuracy & loss curves.
- Comparison: Speed vs accuracy trade-offs across recurrent models.

## 📊 Visualizations

- Token distribution plots
- Training vs validation curves (loss & accuracy)
- Final comparison of model performance

## 🎯 Impact

This project provides insights into:

- Which recurrent architectures best capture text dependencies.

- Trade-offs between accuracy, complexity, and computational cost.

- Applicability in text classification, sentiment analysis, and NLP pipelines.

## 📝 Citation

If you use this work, please cite:
Bhavika Prasannakumar (2025). Exploring RNNs, LSTMs, and GRUs with Embedding Layers on Text Data. GitHub repository: https://github.com/bhavika28/rnn-text-classification
