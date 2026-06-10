## Next Word Prediction using LSTM

A Natural Language Processing (NLP) project that predicts the next word in a sentence using Long Short-Term Memory (LSTM) networks. The model is trained on the HuffPost News Category Dataset and learns contextual relationships between words to generate meaningful text continuations.

## Features

* Text preprocessing and cleaning
* Tokenization using TensorFlow/Keras Tokenizer
* Sequence generation for language modeling
* Word embeddings using Embedding Layer
* LSTM-based next-word prediction
* Text generation from user-provided seed text

## Dataset

This project uses the **News_Category_Dataset_v3** (HuffPost News Dataset).

The model is trained on:

* News Headlines
* Short Descriptions

A sample of 20,000 news articles is used for training.

## Model Architecture

Input Layer
↓
Embedding Layer (100 dimensions)
↓
LSTM Layer (150 units)
↓
Dense Output Layer (Softmax)

## Technologies Used

* Python
* TensorFlow / Keras
* NumPy
* Pandas

## Training

```bash
Epochs: 20
Batch Size: 256
Loss Function: Sparse Categorical Crossentropy
Optimizer: Adam
```

## Results

The model learns contextual word patterns from news articles and can generate plausible next-word predictions from a given seed phrase.

Example:

Input:

```text
donald trump
```

Output:

```text
donald trump said he would not be ...
```

(The output varies depending on training.)

## Project Structure

```text
├── News_Category_Dataset_v3.json
├── next_word_predictor.py
├── requirements.txt
└── README.md
```

## Future Improvements

* Bidirectional LSTM
* Stacked LSTM architecture
* Attention Mechanisms
* Transformer-based Language Models
* Larger training corpus
* Hyperparameter optimization

## Author

Raj Gupta
