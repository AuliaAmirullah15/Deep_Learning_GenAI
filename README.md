# Deep Learning Projects
This repo contains projects related to Deep Learning (including Generative AI). There are three projects at the moment in this repo such as a Cycle GAN model to transform human images to cat/ dog faces, a generative language model to produce a story and a bird classification that can categorize a bird into 200 species based on the trained model. 

## A. Cycle GAN: Transforming Images with Precision
LINK: https://colab.research.google.com/drive/1KrbEkLGw6WqUf24_qQc7nljjny1OeFko?usp=sharing
### Data Processing
1. Navigating the designated directory with a purpose
2. Streamlining images with random flips, resizing (100x100), and normalization (-1 to 1)
3. Pragmatic choice of 2000 training and 1000 testing images for efficiency
### Model Building
1. Constructing essential blocks for Cycle-GAN generators and discriminators
2. Creating generators, discriminators, and overarching models
3. Implementing periodic image capture through callbacks
4. Defining loss functions for precise adversarial evaluation
### Training Highlights and Interruption
1. Halting at 71 epochs due to Google Colab constraints
2. Acknowledging promising checkpoints at 69 and 70
3. Speculating on the potential improvements if uninterrupted


## B. Fine-Grained Classification: Decoding Avian Diversity
LINK: https://colab.research.google.com/drive/1_1rfIaj1e4pC7dsyM93vwGN2Xnxap_14?usp=sharing
### Data Organization
1. Forming a dataframe from four TXT files
2. Dividing the dataset into training, validation, and test sets
3. Strategically marking training images with a regal "1"
### Model Architecture and Optimization
1. Employing Inception V3 for pretrained efficiency
2. Extracting weights and applying global average pooling 2D
3. Trimming layers, connecting threads to a 512-node hidden layer
4. Opting for Adam with a learning rate starting at 0.001 and decaying gradually
### Fine-Tuning Tactics and Achievements
1. Adjusting 300 layers through unfreezing and SGD optimization
2. Attaining a noteworthy 55% accuracy by inheriting wisdom from epochs 30 to 40


## C. Language Model: Unveiling N-Gram Predictions
LINK: https://colab.research.google.com/drive/1gu8Woy6S3QUBq5p6bKih5yjSMW7ONVum?usp=sharing
### Text Preprocessing
1. Reading text by lines, appending to an array
2. Removing punctuations and assembling sentences into an array
3. Utilizing N-Gram for sequence-based word predictions
### Model Development Steps
1. Tokenizing sentences for foundational structure
2. Generating padding sequences, predictor, and target variables
3. Implementing an LSTM network with 100 nodes and 20% dropout
4. Applying softmax with input based on word length
