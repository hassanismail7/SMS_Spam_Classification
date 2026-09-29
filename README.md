# SMS Spam Classification

This project builds an SMS spam classifier in the `spamclassification.ipynb` notebook.

## Setup

Install the required Python packages:

pip install numpy torch scikit-learn datasets gdown

The project uses the following main libraries:

NumPy — numerical operations and embedding matrices
PyTorch — building and training the neural networks
scikit-learn — model evaluation and classification metrics
Hugging Face Datasets — loading the SMS Spam Collection dataset
gdown — downloading the GloVe embedding file

## Run

Open `spamclassification.ipynb` in Jupyter Notebook or VS Code and run the cells in order. The notebook downloads the `ucirvine/sms_spam` dataset and creates an 80/20 train-test split.

## Data Files

`glove_vectors.txt` contains local word-vector data and is intentionally excluded from version control.

## Overall Flow

The project follows this NLP pipeline:

SMS Messages
    ↓
Tokenization
    ↓
Vocabulary Building
    ↓
Word-to-ID Conversion
    ↓
Pretrained GloVe Embeddings
    ↓
Embedding Matrix
    ↓
PyTorch Dataset & DataLoader
    ↓
Padding Variable-Length SMS
    ↓
RNN / GRU / LSTM
    ↓
Linear Classification Layer
    ↓
Spam / Not Spam

## Data Files

glove_vectors.txt contains local pretrained word-vector data and is intentionally excluded from version control.