# NLP-Text-Based-Metrics-Image-Captioning
Generating Captions for Images using NLP and Bleu metrics.

OBJECTIVE:
The main objective of the project is to evaluate a Natural Language Processing  System by applying various text based metrics

ABSTRACT:
When we are trying to solve real world NLP problems, we would want to know the model’s performance on these tasks, 
to make an informed decision, to be aware of the trade-offs we are making. This is where the goodness of a metric comes in. 
The real world is full of biases and we don’t want our solutions to be biased as it can have inconceivable consequences.
So we are applying various text based metrics like WER, BLUE, GLUE, METEOR, TER, ROUGE, CIDEr on our NLP system to evaluate it. 

PROPOSED SYSTEM:

The basic working of the project is that the features are extracted from the images using pre-trained VGG16 model and 
then fed to the LSTM model along with the captions to train. The trained model is then capable of generating captions for any images that are fed to it.
The dataset used here is the FLICKR 8K which consists of around 8091 images along with 5 captions for each images. 

The following are the Dependencies needed for the project:Keras, Tensorflow GPU, Pre-trained VGG-16 weights, NLTK, Matplotlib

SUMMARY OF METRICS USED:

Word Error Rate (WER)  
• Levenshtein distance: edit distance 
• > 0 when ref=hyp
• (S+D+I)/N = (S+D+I)/(S+D+C) 

GENERAL BLEU:

Closer to human judgments than BLEU 
Computes n-gram precisions over the reference and assigns more weight to n-grams that have been correctly changed from the source

GOOGLE BLEU:

Minimum of BLEU recall and precision applied to 1, 2, 3 and 4 grams 
Similar performance to BLEU on corpus level as well as sentence level 

CONCLUSION:
The model has been successfully trained to generate the captions as expected for the images.
The caption generation has constantly been improved by fine tuning the model with different hyper parameter. 
Higher BLEU score indicates that the generated captions are very similar to those of the actual caption present on the images. 



