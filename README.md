
---

# Shakespearean Text Generation with RNN

This project uses a Recurrent Neural Network (RNN) to generate text that emulates the style of William Shakespeare. Built with TensorFlow and Keras, the model learns from sequences of characters in Shakespeare’s works to predict the next character, resulting in generated text with Shakespearean language characteristics.

## Project Summary

- **Objective**: Generate text resembling Shakespeare's writing style.
- **Model Architecture**:
  - **Embedding Layer**: Converts characters into dense vector representations.
  - **RNN Layer**: Processes sequential character data, capturing language patterns.
  - **Output Layer**: Uses softmax activation to predict the probability of each character.

## Dataset

- **Source**: Collection of Shakespeare’s works.
- **Format**: Character sequences, structured for next-character prediction.
- **Preprocessing**: Each input sequence is paired with a target sequence offset by one character, helping the model learn character dependencies.

## Training Details

- **Loss Function**: Sparse Categorical Crossentropy, suitable for character-level classification.
- **Epochs**: Trained for 10 epochs, with checkpoints saved at each stage.
- **Training Progress**: Loss decreased from 3.06 at Epoch 1 to 1.15 at Epoch 10, indicating effective model learning.

## Text Generation

- **Process**: Generates text character-by-character, controlled by a temperature parameter to adjust randomness.
- **Sample Output** (Seed: "ROMEO:"):
  ```
  ROMEO:
  Thou say, none as first loed of! Gentle king,
  Where pretty time without mine: you are full of twate
  ```

###  Contact 
