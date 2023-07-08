## RNN binary classification
This is a basic RNN classification using tensorflow. In this notebook, you will find a basic RNN model.

## Data
The data is from kaggle basic NLP competition. https://www.kaggle.com/competitions/nlp-getting-started/overview


## Model Architecture
### TextVectorization Layer:
Converts input text into integer-encoded sequences using a predefined vocabulary.
### Embedding Layer:
Maps the integer-encoded sequences to dense vector representations.
#### Input dimension: Size of the vocabulary obtained from the TextVectorization layer.
#### Output dimension: 64 (configurable).
Mask zero: True (to handle variable sequence lengths).
### Bidirectional LSTM Layer:
Processes the embedded sequences bidirectionally, capturing contextual information.
Number of units: 64 (configurable).
### Dense Layers:
Fully connected layers to learn non-linear relationships in the data.
Number of units: 64, 32, 16 (configurable).
### Output Layer:
Dense layer with a sigmoid activation function to predict the probability of the positive class.

### Training Details
Loss Function: Binary Crossentropy<br>
Optimizer: Adam (learning rate: 0.001)<br>
Batch Size: Configurable<br>
Number of Epochs: 20 (configurable)<br>
Validation Data: Utilizes a separate test dataset<br>
Metrics: Accuracy

### References
Official RNN text classification tutorial by Tensorflow<br>
https://www.tensorflow.org/text/tutorials/text_classification_rnn<br><br>

Kaggle Discussion - Best NLP Kernels For Beginners<br>
https://www.kaggle.com/competitions/nlp-getting-started/discussion/134890
