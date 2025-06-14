Fake News Detection Using Deep Learning (BiLSTM, LSTM, RNN)

-Project Objective-
This project aims to accurately classify political statements as fake or real using Natural Language Processing (NLP) and Deep Learning. We use the LIAR dataset, build multiple sequence-based neural network models (RNN, LSTM, BiLSTM), and deploy the best-performing model using a simple Flask web interface.

-Tech Stack-
- Python
- TensorFlow / Keras
- BiLSTM, LSTM, RNN
- Flask (Web Deployment)
- GloVe Word Embeddings
- Pandas, NumPy, scikit-learn
- Matplotlib / Seaborn (Visualization)
- Jupyter Notebooks

-Dataset – LIAR-

- 12,836 short statements labeled by PolitiFact editors.
- Labels: `true`, `mostly-true`, `half-true`, `barely-true`, `false`, `pants-fire`
- Converted to binary classification:
  - `1` → true / mostly-true
  - `0` → all others

-Models Built-

| Model   | Description                          | Performance |
|---------|--------------------------------------|-------------|
| RNN     | Simple sequential processing         | ~72%        |
| LSTM    | Captures long-term dependencies      | ~79%        |
| BiLSTM  | Bidirectional context, best performer| 83.5%       |

All models used:
- 100D GloVe Embeddings
- Padding to fixed sequence length
- Dropout regularization
- Adam optimizer with binary cross-entropy loss

-Web App Preview-

An interactive Flask app (`webapp.ipynb`) allows users to input any political statement and get an instant prediction:  
> “Fake” or “Real”

```bash
# To run locally
pip install flask tensorflow
python webapp.ipynb

-Skills-
`TensorFlow`, `Keras`, `Flask`, `scikit-learn`, `Python`, `Pandas`, `NumPy`, `Matplotlib`, `BiLSTM`, `LSTM`, `RNN`, `Binary Classification`, `Text Classification`, `GloVe Embeddings`, `Tokenization`, `Padding`, `EarlyStopping`, `train_test_split`
