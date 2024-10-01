# Exploring Recurrent Neural Networks(RNN, LSTMs and GRUs) with Embedding Layers on Text Data

### Steps for the Project:

#### Step 1: Load and Preprocess the Dataset
- Load the provided text dataset from the Jupyter notebook.
- Keep only the 10,000 most frequent words.
- Convert the text data into sequences of integers where each word is represented by its integer index.
- Split the dataset into training, validation, and test sets.

---

### Task 1: Vanilla RNN Implementation

#### Step 2: Add Embedding Layer
- Add an **Embedding Layer** as the first layer of the network with the following parameters:
  - `embedding_dim=64`
  - `input_dim=10000` (for Keras) or `num_embeddings=10000` (for PyTorch).

#### Step 3: Vanilla RNN (Hidden Dimension = 64)
**1a. Vanilla RNN with Sigmoid Activation**
- Implement a Vanilla RNN with:
  - **hidden dimension=64**
  - Follow it with a fully connected (FC) layer with **1 neuron** and **sigmoid activation**.

**1b. Vanilla RNN with Global MaxPooling and ReLU Activation**
- Implement the Vanilla RNN with:
  - **hidden dimension=64**
  - Add a **Global MaxPooling 1D** layer.
  - Add an FC layer with **16 neurons** and **ReLU activation**.
  - Add another FC layer with **1 neuron** and **sigmoid activation**.

#### Step 4: Performance Evaluation for Vanilla RNN
- Train both models and report the **test accuracy**.
- Plot:
  - **Training Loss vs Validation Loss**
  - **Training Accuracy vs Validation Accuracy**

---

### Task 2: LSTM Implementation

#### Step 5: LSTM (Hidden Dimension = 64)
**2a. LSTM with Sigmoid Activation**
- Implement an LSTM model with:
  - **hidden dimension=64**
  - Follow it with an FC layer with **1 neuron** and **sigmoid activation**.

**2b. LSTM with Global MaxPooling and ReLU Activation**
- Implement the LSTM with:
  - **hidden dimension=64**
  - Add a **Global MaxPooling 1D** layer.
  - Add an FC layer with **16 neurons** and **ReLU activation**.
  - Add another FC layer with **1 neuron** and **sigmoid activation**.

**2c. Stacked LSTM with Global MaxPooling and ReLU Activation**
- Stack two LSTM layers with:
  - **hidden dimension=64** for both layers.
  - The output of the stacked LSTM layers should go to a **Global MaxPooling 1D** layer.
  - Add an FC layer with **16 neurons** and **ReLU activation**.
  - Add another FC layer with **1 neuron** and **sigmoid activation**.

#### Step 6: Performance Evaluation for LSTM
- Train the models (2a, 2b, 2c) and report the **test accuracy**.
- Plot:
  - **Training Loss vs Validation Loss**
  - **Training Accuracy vs Validation Accuracy**

---

### Task 3: GRU Implementation

#### Step 7: GRU (Hidden Dimension = 64)
**3a. GRU with Sigmoid Activation**
- Implement a GRU model with:
  - **hidden dimension=64**
  - Follow it with an FC layer with **1 neuron** and **sigmoid activation**.

**3b. GRU with Global MaxPooling and ReLU Activation**
- Implement the GRU with:
  - **hidden dimension=64**
  - Add a **Global MaxPooling 1D** layer.
  - Add an FC layer with **16 neurons** and **ReLU activation**.
  - Add another FC layer with **1 neuron** and **sigmoid activation**.

#### Step 8: Performance Evaluation for GRU
- Train the models (3a, 3b) and report the **test accuracy**.
- Plot:
  - **Training Loss vs Validation Loss**
  - **Training Accuracy vs Validation Accuracy**
