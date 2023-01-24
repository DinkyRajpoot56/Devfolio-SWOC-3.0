1) Multilayer Perceptrons (MLPs)
MLP is the most basic deep learning algorithm and also one of the oldest deep learning techniques. If you are a beginner in deep learning and have just started exploring it, we recommend you get started with MLP. MLPs can be referred to as a form of Feedforward neural networks. 

How does MLP deep learning algorithm work?
The working of MLP is the same as what we discussed above in our MNIST data example. The first layer, namely the input layer, takes the inputs, and the last layer produces the output based on the hidden layers. Each node is connected to every node on the next layer, so the information is constantly fed forward between the multiple layers, which is why it is referred to as a feedforward network.

MLP uses a prevalent supervised learning technique called backpropagation for training.

MLP deep learning algorithm

 

Each hidden layer is fed with some weights (randomly assigned values). The combination of the weights and input is supplied to an activation function which is passed further to the next layer to determine the output. If we don’t arrive at the expected output, we calculate the loss (error) and back-track to update the weights. It is an iterative process until the predicted output is obtained (trial and error). It is critical in training the deep learning model, as the correct weights will determine your final output.

MLPs popularly use sigmoid functions, Rectified Linear unit (ReLU), and tanh as activation functions.

With these Data Science Projects in Python, your career is bound to reach new heights. Start working on them today!

Applications of MLP 
It is used by Social media sites (Instagram, Facebook) for compressing image data. That significantly helps to load the images even if the network strength is not too strong.

Other applications include Usage in image and speech recognition, data compression, and also for solving classification problems.

Pros of MLP 
They do not make any assumptions regarding the Probability density functions (PDF), unlike the other models that are based on Probability.

Ability to provide the decision function directly by training the perceptron.

Cons of MLP 
 Due to the hard-limit transfer function, the perceptrons can only give outputs in the form of 0 and 1. 

 While updating the weights in layers, the MLP network may be stuck in a local minimum which can hamper accuracy. 

2) Radial Basis Function Networks (RBFNs)
As the name suggests, it is based on the Radial basis function (RBF) activation function. This deep learning method training process requires slightly less time using RBFN than MLP. 

How do RBFN deep learning algorithms work?
A straightforward type of RBFN is a three-layer feedforward neural network with an input layer, a hidden layer consisting of several RBF nonlinear activation units, and a linear output layer that acts as a summation unit to give the final output.

RBFN deep learning algorithm

 

RBFN uses trial and error to determine the structure of the network. That is done in two steps -

In the first stage, the centers of the hidden layer using an unsupervised learning algorithm (k-means clustering) are determined.

In the next step, the weights with linear regression are determined. Mean Squared Error (MSE) is used to determine the error, and the weights are tweaked accordingly to minimize MSE.

Explore Categories

Machine Learning Projects in Python Machine Learning Projects in R Deep Learning Projects Neural Network Projects Tensorflow Projects H2O R Projects IoT Projects Keras Deep Learning Projects NLP Projects Pytorch Data Science Projects in Banking and Finance Data Science Projects in Retail & Ecommerce Data Science Projects in Entertainment & Media Data Science Projects in Telecommunications
Applications of RBFN  
RBFNs are used to analyze stock market prices and forecast sales prices in Retail industries because of their ability to work on time-series-based data. Other applications include Speech recognition, time-series analysis, image recognition, adaptive equalization, medical diagnosis, etc.

Pros of RBFN
1) The training process is faster when compared to MLP, as there is no backpropagation involved.

2) It is easy to interpret the roles of the hidden layer nodes compared to MLP.

Cons of RBFN 
Although we have seen that the training is faster in the RBF network, classification takes time as compared to Multilayer Perceptrons. 

The reason is that every node in the hidden layer must compute the RBF function for the input sample vector during classification.

It is easy to interpret the roles of the hidden layer nodes compared to MLP.

Cons of RBFN

Input and output for the RBFN deep learning model

We want our model to recognize the objects irrespective of what surface they are upon and their position. 

3) Convolutional Neural Networks (CNN)
In CNN, the processing of data involves breaking the images into many numbers of overlapping tiles instead of feeding entire images into our network. And then, we use a technique called a sliding window over the whole original image and save the results as a separate tiny picture tile. The Sliding window is a kind of brute force solution where we scan all around for a given image to detect the object for all possible sections, each section at a time until we get the expected object.

How do CNN deep learning algorithms work?
There are three basic building blocks of a CNN

Convolutional layers

Pooling layers

Full-Connected Layers

Unlock the ProjectPro Learning Experience for FREE

CNN deep learning algorithms

Image source - Wikipedia

Convolutional Layer – It is the most significant building block of convolutional neural networks. A set of filters (kernels) are used in the layer’s parameters that can be visualized as neurons of the layers. They have weighted inputs and based on the input size (a fixed square) that is also referred to as a receptive field; they provide the output.

These filters, when applied to the input image, generate feature maps. It is the output of one filter that is applied to the previous layer. Moving one image pixel at a time, a given filter is drawn across the entire previous layer. For each position, a particular neuron is activated, and the output is collected in a feature map. 

Convolutional Layer

 

To avoid losing the arrangement of the original image tiles, we save the result obtained after processing each tile into a grid with the same tiles' arrangement as the original image.

Pooling Layer- In the convolution layer, the output is a grid array huge in size. To reduce the size of this array, we use an algorithm max pooling for down-sampling. The basic idea of using a pooling layer is to keep only the most significant input tile from the array.

Fully connected Layer – The array is only a bunch of numerical values, so we can input them into a neural network that is fully connected (all neurons are connected). CNN most commonly uses ReLU as the activation function.

Applications of CNN
Social Media sites like Facebook, Instagram, etc., use CNNs for face detection and recognition. So when trying to tag your friend in your post, you are using CNN!

Other applications include Video analysis, Image recognition, Natural language processing, Forecasting, etc.

Pros of CNN
CNN results are more accurate, particularly for image/object recognition use cases, compared to other algorithms.

Cons of CNN
High computation power is required for training CNNs. So, they are not cost-effective.

Get confident to build end-to-end projects.

Access to a curated library of 250+ end-to-end industry projects with solution code, videos and tech support.

4) Recurrent Neural Networks (RNNs)
Have you noticed when you start typing something, Google automatically completes the sentence for you! Now, if you are thinking about how it works, the secret is RNN.

Recurrent Neural Networks have directed cycles among the interconnected nodes. They use their memory to process the next sequence of inputs to implement the auto-complete feature kind of functionalities. RNNs can take a series of inputs with no limit on their size, making them unique. 

How do RNN deep learning algorithms work?
RNN deep learning algorithms

 

The Basic Structure of RNN
The above figure shows the different steps for each time state for a recurrent neural network. RNNs do not only account for the weights of hidden units to determine the output but also use the information learned from their prior inputs. RNNs are a special type of deep neural network that can remember those characters because of their internal memory. An output is produced, which is copied and provided back to the deep neural network like a loop. That is why the input could produce a different output based on previous inputs in the connected layers.

Let us understand this by an example -

Example - Imagine if you have built a feedforward network that takes words as input and processes the word character by character. You pass the word ProjectPro, and by the time you reach the character "o", it would have already forgotten the last characters "P," "r", and "o". 

Applications of RNN
Google, Search Engines, and Web Browsers extensively use RNN to auto-complete words and sentences. Other applications are Text Detection and Recognition, Analyzing video frames, etc.

Pros of RNN  
The ability of RNN models to remember information throughout the training period plays a pivotal role in time series prediction.

Cons of RNN  

The computation is time-taking because of its recurrent nature.

 Hard to process long sequences in the training data set, mainly when we use ReLU or tanh as activation functions.

5) Long Short-Term Memory Networks (LSTMs)
LSTMs are a special kind of RNN and are highly capable of learning long-term dependencies. Let’s try to understand long-term dependencies by an example.

Suppose you have built a model to predict the next word based on the previous ones. Assume you are trying to predict the last word in the sentence, “the sun rises in the east,” we don’t need any further context, and obviously the following term will be east. In these types of cases, where there is not much gap between the relevant information and the place where it’s needed, RNNs can learn and predict the output easily. But if we have a sentence like, “I am born in India. I speak fluent Hindi”. This kind of prediction requires some context from the previous sentence about where a person was born, and RNNs might not be able to learn and connect the information in such cases.

How do LSTM deep learning algorithms work?
LSTM deep learning algorithms

 

The LSTM network consists of different memory blocks called cells(the rectangular blocks above).  

The cell state and hidden state are transferred to the next cell.  As the name suggests, memory blocks remember things, and the changes to these memory blocks are done through mechanisms referred to as gates. 

The key to LSTMs is the cell state (the horizontal line at the top, which runs through in the diagram). 

The key to LSTMs is the cell state (the horizontal line at the top which runs through in the diagram). 

Step 1: -  LSTM decides what information should be kept intact and what should be thrown away from the cell state. The sigmoid layer is responsible for making this decision.

Step 2: - LSTM decides what new information one should keep and replaces the irrelevant one identified in step 1 - the tanh and the sigmoid function play an important role in identifying relevant information.

Step 3: - The output is determined with the help of the cell state that will now be a filtered version because of the applied sigmoid and tanh functions.

Applications of LSTM
Anomaly detection in network traffic data or IDSs (intrusion detection systems), Time-series forecasting, Auto-completion, text and video analysis, and Caption generation. 

Pros of LSTM
LSTMs when compared to conventional RNNs, are very handy in modeling the chronological sequences and long-range dependencies. 

Cons of LSTM
High computation and resources are required to train the LSTM model, and it is also a very time-consuming process.

They are prone to overfitting.

6) Restricted Boltzmann Machines (RBMs)
RBM is one of the oldest algorithm in deep learning invented in 1986 by Geoffrey Hinton. I bet you would have noticed how YouTube recommends videos similar to what you have watched recently. Also, if you have watched a web series or movie on Netflix, you will start getting a lot of recommendations related to them. They use a technique known as collaborative filtering that uses RBMs.

Get FREE Access to Data Analytics Example Codes for Data Cleaning, Data Munging, and Data Visualization

How do RBM deep learning algorithms work?
RBM deep learning algorithms

 

RBM for a single input

RBM is one of the simplest deep learning algorithms and has a basic structure with just two layers-

(Visible) Input layer

Hidden layer

The input x is multiplied by the respective weight(w) at each hidden node. A single input x can have 8 weights altogether (2 input nodes x 4 hidden nodes). The hidden nodes receive the inputs multiplied by their respective weights and a bias value. The result is passed through an activation function to the output layer for reconstruction. RBMs compare this reconstruction with the original input to determine the quality of the result. If the quality of the result is not good, the weights are updated, and a new reconstruction is built. 

Applications 
Netflix, Prime Video, and Streaming apps provide recommendations to users based on their watching patterns using the RBM algorithm.

Feature extraction in pattern recognition, Recommendation Engines, Classification problems, Topic modeling, etc.

Pros of RBM 
RBMs can be pre-trained in a completely unsupervised way as the learning algorithm can efficiently use extensive unlabelled data.

They don’t require high computation and can encode any distribution.

Cons of RBM  
Calculation of energy gradient function while training is challenging.

Adjusting weights using the CD-k algorithm is not as easy as backpropagation.

7) Self-Organizing Maps (SOMs)
Imagine you are working with a dataset with hundreds of features, and you want to visualize your data to understand the correlation between each feature. It is not possible to imagine it using scatter or pair plots. Here comes SOMs. It reduces the data's dimension (less relevant features are removed) and helps us visualize the distribution of feature values.

How does the SOM deep learning algorithm work?
SOMs group similar data items together by creating a 1D or 2D map. Similar to the other algorithms, weights are initialized randomly for each node. At each step, one sample vector x is randomly taken from the input data set and the distances between x and all the other vectors are computed.

A Best-Matching Unit (BMU) closest to x is selected after voting among all the other vectors. Once BMU is identified, the weight vectors are updated, and the BMU and its topological neighbors are moved closer to the input vector x in the input space. This process is repeated until we get the expected output.

SOM deep learning algorithm

 

For our example, the program would first select a color from an array of samples, such as red, and then search the weights for those red locations. The weights surrounding those locations are red, and then the next color, blue is chosen, and the process continues.

Applications
Image analysis, fault diagnosis, process monitoring, and control, etc. SOMs are used for 3D modeling human heads from stereo images because of their ability to generate powerful visualizations, and they are extensively valuable for the healthcare sector for creating 3D charts.

Pros of SOMs  
We can easily interpret and understand the data using SOM. 

Using dimensionality reduction further makes it much simpler to check for any similarities within our data.

Cons of SOMs 
SOM requires neuron weights to be necessary and sufficient to cluster the input data. 

If, while training SOM, we provide less or extensively more data, we may not get the informative or very accurate output.

8) Generative Adversarial Networks (GANs)
It is an unsupervised learning algorithm capable of automatically discovering and learning the patterns in the data. GANs then generate new examples that resemble the original dataset.

How do GAN deep learning algorithms work?
GANs consist of two neural networks.

Generator Network - First is a generator neural network that generates new examples.

Discriminator Network – It is responsible for evaluating the generated examples and whether they belong to the actual training dataset.

GAN deep learning algorithms

Credits-O’Reilly

Let us understand this by an example. Consider a currency note checking machine. The machine is responsible for checking if the notes are fake or real. The Generator network will try to create counterfeit notes and send them to the Discriminator. The Discriminator will take in both the real (input training data) and the fake notes and return a value between 0 to 1. This value is a probability where 1 represents completely genuine notes and 0 represents fake notes. 

Both Generator and Discriminator will try to outperform each other and get trained at the same time. 

Applications of GANs
GANs are widely used in the gaming industry for 3D object generations. They are also used for editing images, generating cartoon characters, etc.

They are also used for illustrations for novels, articles, etc.

Pros of GANs 
GANs can learn any data's internal representation (messy and complex distributions). They can be trained effectively using unlabeled data so they can quickly produce realistic and high-quality results.

They can recognize objects as well as can calculate the distance between them.

Cons of GANs 
As they generate new data from original data, there is no such evaluation metric to judge the accuracy of output.

High computation and time required for model training.

9) Autoencoders Deep Learning Algorithm
Autoencoders are unsupervised algorithms very similar to Principal Component Analysis (PCA) in machine learning. They are used to convert multi-dimensional data into low-dimensional data. And if we want the original data, we can regenerate it back.

A simple example is -Suppose your friend has asked you to share a software you have saved on your computer. The folder size of that software is close to 1 GB. If you directly upload this whole folder to your Google drive, it will take a lot of time. But if you compress it, then the data size will reduce, and you can upload it easily. Your friend can directly download this folder, extract the data, and get the original folder.

In the above example, the original folder is the input, the compressed folder is encoded data, and when your friend extracts the compressed folder, it is decoding.

How do autoencoders work?
There are 3 main components in Autoencoders – 

Encoder – The encoder compresses the input into a latent space representation which can be reconstructed later to get the original input.

Code – This is the compressed part (latent space representation) that is obtained after encoding.

Decoder – The decoder aims to reconstruct the code to its original form. The reconstruction output obtained may not be as accurate as the original and might have some loss.

autoencoders work

 

The code layer present between the encoder and decoder is also referred to as Bottleneck. It is used to decide which aspects of input data are relevant and what can be neglected. The bottleneck is a very significant layer in our network. Without it, the network could easily learn to memorize the input values by passing them along through the network.

Applications
Colouring of images, image compression, denoising, etc.

They are used in the healthcare industry for medical imaging (technique and process of imaging the human body's interior for performing clinical analysis)  Eg - breast cancer detection.

Pros of Autoencoders
Using multiple encoder and decoder layers reduces the computational cost of representing some functions to a certain extent.

Cons of Autoencoders  
It is not as efficient as GANs when reconstructing images as for complex images,it usually does not work well.

We might lose essential data from our original input after encoding.

10) Deep Belief Networks
A deep belief network (DBN) is built by appending several Restricted Boltzmann Machines (RBM) layers.  Each RBM layer can communicate with both the previous and subsequent layers.

DBNs are pre-trained by using the Greedy algorithm. It uses a layer-by-layer approach to learn all the generative weights and the top-down approaches. The weights associated determine how all variables in one layer rely on the other variables in the above layer.

How do deep belief networks work?
DBNs are pre-trained by using the Greedy algorithm. They use a layer-by-layer approach to learn all the generative weights and the top-down approaches. The weights associated determine how all variables in one layer rely on the other variables in the above layer.

Several steps of Gibbs sampling (for obtaining a sequence of observations approximated from a specified multivariate probability distribution when direct sampling is difficult) are run on the top two hidden layers of the network. The idea is to draw a sample from the RBM defined by the top two hidden layers.

In the next step, we use a single pass of ancestral sampling through the rest of the model to draw a sample from the visible units.

A single, bottom-up pass can conclude learning the values of the latent variables in every layer. 

The Greedy pre-training starts with an observed data vector in the lowest layer. Then it uses the generative weights in the opposite direction with the help of fine-tuning.

deep belief networks

Applications
Variational Autoencoder(VAE), a type of autoencoder is used to generate anime characters in the entertainment/gaming industry

 To recognize, cluster, and create images, video sequences, and motion-capture data. 

Pros of DBNs 
They can work with even a tiny labeled dataset.

DBNs provide robustness in classification. (view angle, size, position, color, etc.)

Cons of DBNS
Hardware requirements are high to process inputs.

Most Watched Projects


Best Deep Learning Algorithms
Before we end this blog on a sweet note, we’d like to highlight some algorithms that work best for particular use cases.

Deep Learning Algorithms for Sentiment Analysis
The best deep learning algorithm for sentiment analysis is Recurrent Neural Network, RNN. That’s primarily because of their recurrent nature that allows them to work with sequential data like text. They are used for analysing the sentiment of each word or token in the text. Once the model has been trained till the end of text, the sentiment prediction is the output of the model after scanning all the n tokens.

Deep Learning Algorithms for Image Processing and Image Classification
Convolutional neural networks (CNNs) are best suited for image processing and image classification problems as the convolution operation allows processing the images with the help of different filter functions. Using different 