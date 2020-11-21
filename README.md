# NLP-Text-Based-Metrics-Image-Captioning
<h2> Generating Captions for Images using NLP and Bleu metrics </h2>

<h3>OBJECTIVE:</h3>

The main objective of the project is to evaluate a Natural Language Processing  System by applying various text based metrics

<h3>ABSTRACT:</h3>

In the past few years, the problem of generating descriptive sentences automatically for images has garnered a rising interest in natural language processing and computer vision research. Image captioning is a fundamental task which requires semantic understanding of images and the ability of generating description sentences with proper and correct structure. In this study, the authors propose a hybrid system employing the use of VCG16 model to generate vocabulary describing the images and a Long Short Term Memory (LSTM) to accurately structure meaningful sentences using the generated keywords. We showcase the efficiency of our proposed model using the Flickr8K datasets and show that their model gives accurate results compared utilising the Bleu metric. The Bleu metric is an algorithm for evaluating the performance of a machine translation system by grading the quality of text translated from one natural language to another. 

<h3>INTRODUCTION:</h3>

Caption generation is an interesting artificial intelligence problem where a descriptive sentence is generated for a given image. It involves the dual techniques from computer vision to understand the content of the image and a language model from the field of natural language processing to turn the understanding of the image into words in the right order. Image captioning has various applications such as recommendations in editing applications, usage in virtual assistants, for image indexing, for visually impaired persons, for social media, and several other natural language processing applications. 

Recently, deep learning methods have achieved state-ofthe-art results on examples of this problem. It has been demonstrated that deep learning models are able to achieve optimum results in the field of caption generation problems. Instead of requiring complex data preparation or a pipeline of specifically designed models, a single end-to-end model can be defined to predict a caption, given a photo. In order to evaluate our model, we measure its performance on the Flickr8K dataset using the BLEU standard metric. These results show that our proposed model performs better than standard models regarding image captioning in performance evaluation. 

<h3>PROPOSED SYSTEM:</h3>

The basic working of the project is that the features are extracted from the images using pre-trained VGG16 model and 
then fed to the LSTM model along with the captions to train. The trained model is then capable of generating captions for any images that are fed to it.
The dataset used here is the FLICKR 8K which consists of around 8091 images along with 5 captions for each images. 

The following are the Dependencies needed for the project:Keras, Tensorflow GPU, Pre-trained VGG-16 weights, NLTK, Matplotlib

<h3>SUMMARY OF METRICS USED:</h3>

Word Error Rate (WER)  
• Levenshtein distance: edit distance 
• > 0 when ref=hyp
• (S+D+I)/N = (S+D+I)/(S+D+C) 

<h3>GENERAL BLEU:</h3>

Closer to human judgments than BLEU 
Computes n-gram precisions over the reference and assigns more weight to n-grams that have been correctly changed from the source

<h3>GOOGLE BLEU:</h3>

Minimum of BLEU recall and precision applied to 1, 2, 3 and 4 grams 
Similar performance to BLEU on corpus level as well as sentence level 

<h3>CONCLUSION:</h3>

The model has been successfully trained to generate the captions as expected for the images.
The caption generation has constantly been improved by fine tuning the model with different hyper parameter. 
Higher BLEU score indicates that the generated captions are very similar to those of the actual caption present on the images. 



