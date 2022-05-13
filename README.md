# EcommerceChatBot

### A brief overview of my process, all found in the Jupyter Notebook:
### 1) I first create a couple of natural language processing functions such as tokenization, stemming and bag of words. These functions are used in most of the following stages of the project.

### 2) I then open up the JSON intents file that contains tags, patterns and response strings that serve as the bread and butter of the training data and potential user inputs with the chatbot. Ecommerce related tags such as "greetings", "products", and "payment methods" can be seen in the file. I then go through the whole file and import all its data into lists to be used later.

### 3) I then created a dataset with the featurs being bag of word strings and labels being the tag the strings belong to. I also split up the data into training and testing with a ratio of 0.2 for testing.

### 4) Next I created my feed forward model using three linear layers with ReLU activation in between and then proceeded to train the data through 500 epochs.

### 5) Next I looked at some metrics and plotted the training loss over time.

### 6) Finally I implemented the loop that is in charge of interacting with the customer. I randomized chatbot names every time the program is run in order to make it feel more sentimental and realistic to the customer and feel like they are speaking to a real person.
