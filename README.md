# Chatbot with Natural Language Processing (NLP)

This is a simple chatbot application built using Natural Language Processing (NLP) techniques. It leverages a trained deep learning model to process and respond to user inputs based on predefined intents. The chatbot is implemented using Python, Keras, and TensorFlow for training and prediction, and NLTK for text processing.

## Features

- **Predictive Text Processing**: The chatbot can predict user intent based on input text.
- **Predefined Responses**: It provides responses by matching user input with a predefined set of intents and patterns.
- **NLP Techniques**: Utilizes tokenization and lemmatization for processing the input sentences.
- **Deep Learning Model**: Uses a neural network to classify intents and predict responses.
- **Interactive**: Users can interact with the chatbot in real-time through a terminal interface.

## Project Structure

```bash
├── main.py                # The main chatbot interface for user interaction
├── training.py            # Script for training the model with intents and patterns
├── intents.json           # JSON file containing intents, patterns, and responses
├── words.pkl              # Saved list of tokenized words
├── classes.pkl            # Saved list of intent classes
├── chatbot_model.h5       # Trained chatbot model
└── README.md              # Project documentation
```

# Getting Started

## Prerequisites

To run this project, you'll need:

- Python 3.x
- Keras and TensorFlow libraries
- NLTK for NLP processing
- MySQL (if database integration is required)

## Setup

### Clone this repository:

```bash
git clone https://github.com/yourusername/chatbot-nlp.git
```

## Install the required Python libraries:

```bash
pip install tensorflow keras nltk numpy
```

## Download necessary NLTK data

Run the following in a Python shell to download the tokenizer and lemmatizer:

```python
import nltk
nltk.download('punkt')
nltk.download('wordnet')
```

## Prepare the Dataset

The chatbot uses `intents.json`, which contains various intents and responses. Modify this file according to your chatbot's requirements.

## Train the Model

To train the model using the defined intents, run the following command:

```bash
python training.py
```

This will create and save the model (`chatbot_model.h5`), along with the necessary word and class files (`words.pkl` and `classes.pkl`).

## Run the Chatbot

Start interacting with the chatbot by running the following command:

```bash
python main.py
```
## Files

- `main.py`: Main interface for the chatbot, allows users to input messages and get a response.
- `training.py`: Script to train the chatbot model using intents and patterns from the `intents.json` file.
- `intents.json`: Contains the intents, patterns (sample phrases for each intent), and corresponding responses.
- `chatbot_model.h5`: Saved Keras model after training.
- `words.pkl`: Tokenized words saved for use during prediction.
- `classes.pkl`: Saved classes (intents) for classification.

## Technologies Used

- **Python**: Programming language used for scripting.
- **Keras & TensorFlow**: Used to build and train the deep learning model.
- **NLTK**: For natural language processing (tokenization and lemmatization).
- **NumPy**: For numerical operations and data manipulation.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- **Keras & TensorFlow** for the deep learning framework.
- **NLTK** for the powerful NLP tools.
- Special thanks to tutorials and online resources for inspiration in building this chatbot.
