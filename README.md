# EcommerceChatBot 🤖

## Project Overivew:
* Created an Ecommerce style Chatbot that interacts with customers inquiring about things like **products, delivery times, and payment methods**
* Built a Json intents file containing various **tags, patterns and responses strings** that I tailored to an Ecommerce environment and used to train and test my model.
* Trained my Chatbot model with a feed forward neural network containing linear input, hidden and output layer with ReLU activation in between layers and a softmax activation for classification.
* Observed metrics such as training loss, accuracy score and f1 score of the model after training.


## A brief overview of my process, all found in the Jupyter Notebook:
1) I first create a couple of natural language processing functions such as **tokenization, stemming and bag of words.** These functions are used in most of the following stages of the project.

2) I then open up the JSON intents file that contains tags, patterns and response strings that serve as the bread and butter of the training data and potential user inputs with the chatbot. Ecommerce related tags such as **"greetings", "products", and "payment methods"** can be seen in the file. I then go through the whole file and import all its data into lists to be used later.

3) I then created a dataset with the featurs being bag of word strings and labels being the tag the strings belong to. I also split up the data into training and testing with a ratio of 0.2 for testing.

4) Next I created my **feed forward model** using three linear layers with ReLU activation in between and then proceeded to train the data through 500 epochs.

| Layer Name & Type | In_Features | Out_Features |
| :---              |:---:        |          ---:|
| l1 linear (input)         | 52          | 8            |
| l2 linear (hidden) | 8 | 8 | 
| l3 linear (output) | 8       | 6|

5) Next I looked at some metrics and plotted the training loss over time.

6) Finally I implemented the loop that is in charge of interacting with the customer. I randomized chatbot names every time the program is run in order to make it feel more sentimental and realistic to the customer and feel like they are speaking to a real person.



Here is a sample convo with the bot!
![Image](https://github.com/akhalifaa/EcommerceChatBot/blob/main/Example%20Convo.png)
