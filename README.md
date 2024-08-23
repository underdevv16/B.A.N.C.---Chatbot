
# B.A.N.C. - A Banking Chatbot

B.A.N.C. stands for Banking Automated Navigation Chatbot.

It is a Banking Chatbot aimed to provide users with answers to their Banking related queries.


## Features:

- Natural Language Understanding: Understands and responds to user queries using a trained neural network model.
- Text-to-Speech Integration: Provides spoken responses to user queries for an interactive experience.
- User-Friendly GUI: Intuitive interface developed with Tkinter for easy interaction.
- Personalized Greetings: Greets users based on the time of day.
- Trained on self acquired data.
## Installation

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/BANC-chatbot.git
```
```bash
cd BANC-chatbot
```
### 2. Install the dependencies
```bash
pip install -r requirements.txt
```
## Overview

- Data Preparation: Collect and prepare data in JSON format with intents, inputs, and responses. This data is used to train the model.
- Model Building: Create a neural network model using TensorFlow and Keras. The model uses an embedding layer, LSTM layers, and a dense output layer to classify input queries and generate responses.
- Training: Train the model with tokenized and padded input data, and save the trained model.
- GUI Development: Develop a graphical user interface using Tkinter. The GUI includes an input field for user queries and a display area for conversation history.
- Integration: Integrate the trained model with the GUI to process user input, predict responses, and utilize text-to-speech for output.
## APIs Used

- TensorFlow: For building and training the neural network model.
- Tkinter: For creating the graphical user interface.
- pyttsx3: For text-to-speech functionality.

## Data Description

The chatbot's responses are powered by a custom dataset stored in a JSON file. This data is structured to train the model to recognize various user inputs and generate appropriate responses.

### Data Structure:

- intents: A list of intent objects, each representing a specific type of user query.
- tag: A label for the intent, such as "greeting" or "howami."
- input: A list of example phrases or questions that users might ask.
- responses: A list of possible replies the chatbot can provide for the given intent.

Example entry:

```bash
{
    "tag": "greeting",
    "input": [
        "hello", "hi there", "nice to meet you", "hi", "hey there", 
        "hey", "hi there", "hi, nice to meet you", "hello there", 
        "anyone there ?", "knock knock"
    ],
    "responses": [
        "Hi there!", "welcome aboard, how may I help you ?", 
        "ahoy!!", "At your service my friend", 
        "Hello my friend, How can I help you ?", 
        "Hi, Glad you are here. How may I assist you ?"
    ]
}

```

### Data Creation:

- The dataset was created manually to cover a range of conversational scenarios. It includes various tags such as greetings, user well-being queries, and more.
- Each intent is crafted with multiple inputs and responses to ensure the chatbot can handle diverse ways of asking the same question and provide varied, contextually appropriate replies.
## Conclusion

B.A.N.C. is a practical example of conversational AI, combining TensorFlow for model training and Tkinter for a user-friendly interface. This project showcases how AI can enhance user interactions in a banking context. Contributions and feedback are welcome as we continue to improve and expand B.A.N.C.

Thank you for exploring B.A.N.C.!
