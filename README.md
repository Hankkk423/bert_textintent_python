# BERT Model for Intent Classification

This project demonstrates intent classification using the DistilBERT model for natural language processing tasks. Intent classification involves categorizing user input into predefined classes or labels, helping to understand user intentions for building chatbots, virtual assistants, and more.

## Overview

Intent classification is an essential part of natural language understanding, particularly in applications where interactions between users and AI systems require accurate interpretation of user input. This project utilizes the DistilBERT model, a lightweight variant of the BERT model, to achieve accurate intent classification.

## Project Features

1. Data Preprocessing: 
The project starts by loading a dataset of user utterances and their corresponding intent labels. The labels are encoded using LabelEncoder, mapping them to numerical values.
2. Tokenizer and Encoding: 
The DistilBERT tokenizer is used to preprocess and tokenize text input. Utterances are encoded into numerical representations with attention masks to indicate actual tokens and padding tokens.
3. Model Architecture: 
The project defines a custom neural network architecture that includes a DistilBERT model followed by fully connected layers. The network is designed to classify the intents present in user utterances.
4. Training Process: 
The model is trained using a training loop, where batches of encoded data are passed through the network. Cross-entropy loss and AdamW optimizer are used for efficient training. Class weights are computed to handle class imbalances.
5. Evaluation and Validation: 
The trained model's performance is evaluated on a validation set. Accuracy metrics are computed to measure both training and validation accuracy, providing insights into the model's performance.
6. Inference and Prediction: 
Once trained, the model is capable of predicting intents for new user input. A custom function, get_prediction, preprocesses and tokenizes the input, then utilizes the trained model to predict the corresponding intent.
7. Visualization: 
Training loss and accuracy trends are visualized over epochs using matplotlib, helping monitor the model's convergence and performance.

## Installation

Before running the code, ensure you have the required packages installed. You can install them using the `requirements.txt` file.

## Usage

1. Clone this repository to your local machine.
2. Install the required packages as mentioned in the installation section.
3. Load and preprocess your dataset, converting text and labels into numerical representations.
4. Configure the model architecture and training settings.
5. Train the model and monitor its performance using the training loss and accuracy plots.
6. Fine-tune the model to achieve better intent classification results.
7. Utilize the trained model to predict intents for new user input.

## Contributing

Contributions to this project are welcome! If you'd like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and test thoroughly.
4. Commit your changes and push them to your fork.
5. Create a pull request to the original repository.

## License

This project is licensed under the MIT License. You can find more details in the LICENSE file.
