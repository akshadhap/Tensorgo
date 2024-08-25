# Tensorgo
We begin by loading an IMDb dataset containing movie reviews labeled as positive or negative, which we'll use to train and test our sentiment analysis model. Using DistilBERT's tokenizer, we convert these text reviews into numbers so the model can understand and process the data. Next, we split the dataset into training and testing sets to evaluate the model's performance. We then load a pre-trained DistilBERT model designed for text classification and fine-tune it for our specific task. During training, we set important parameters like batch size and the number of training cycles, allowing the model to learn to classify reviews accurately. After training, we evaluate the model’s performance by checking its accuracy before and after fine-tuning. We also plot the training loss and validation accuracy to visualize how the model improves over time. Finally, we compare the model's accuracy before and after fine-tuning to demonstrate the effectiveness of the training process.

Loading the IMDb Dataset: We start by loading a dataset from IMDb, which has movie reviews labeled as either positive or negative. This dataset will be used to train and test our sentiment analysis model.

Tokenizing the Text: Next, we use a tokenizer from DistilBERT, a smaller version of the BERT model, to turn the text reviews into numbers. This step is essential because it allows the model to understand and process the data.

Preparing the Data: We then split the dataset into two parts: one for training the model and one for testing it. This helps us to train the model and later check how well it performs.

Model Setup: We load a pre-trained DistilBERT model that's designed for tasks like classifying text. Although the model already has some knowledge, we need to fine-tune it to work better for our specific task.

Training the Model: We set up the training process by defining important parameters like batch size, the number of training cycles (epochs), and how we want to evaluate the model's progress. The Trainer class manages the training, helping the model learn to classify reviews as positive or negative.

Evaluating Performance: After training, we check how well the model is doing by measuring its accuracy. We compare its performance before and after fine-tuning to see how much it has improved.

Visualizing Results: We then plot graphs showing how the model's training loss and validation accuracy change over time. This gives us a visual idea of how well the model is learning during the training process.

Comparison: Finally, we compare the accuracy of the model before and after fine-tuning to highlight the improvements made through the training process.
