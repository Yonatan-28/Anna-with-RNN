# Anna with RNN

This project trains a character-level RNN (LSTM) in PyTorch to generate text in the style of the input corpus. The notebook walks through loading the raw text, encoding characters, batching sequences, training the model, saving a checkpoint, and sampling new text from the trained network.

## What is inside
- A full training pipeline: one-hot encoding, mini-batching, training loop, and validation loss reporting.
- A `CharNN` model using a multi-layer LSTM with dropout.
- Checkpoint save/load to resume or reuse trained weights.
- Text generation by sampling the next character with optional top-k filtering.

## Data
- The training corpus is in [Anna.txt](Anna.txt).

## How to run
1. Open and run the notebook in order: [Training-with-RNN.ipynb](Training-with-RNN.ipynb)
2. Adjust hyperparameters like `n_hidden`, `n_layer`, `batch_size`, `seq_len`, and `epoch` inside the notebook.
3. After training, a checkpoint file (for example, `CheckPoint_20.pth`) is written to the workspace.
4. Run the sampling cell to generate text from the trained model.

## Output
- Training prints per-epoch train/validation loss.
- Sampling prints a generated text string based on the prime prompt.
