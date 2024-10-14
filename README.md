# Image Captioning Project

## Overview
Image captioning involves generating descriptive textual representations of images. The challenge lies in building a model that not only understands the visual content but also expresses it in coherent language. This project leverages **LSTM networks** to generate captions that accurately describe images from the **Flickr8k dataset**.

## Features
- Generates meaningful captions using deep learning.
- Uses the **Flickr8k dataset** for training and evaluation.
- Employs the **VGG16 model** for feature extraction from images.
- Utilizes **LSTM architecture** for natural language generation.
- Evaluates model performance using **BLEU-1** and **BLEU-2** metrics.

## Dataset
This project uses the Flickr8k dataset consisting of 8,000 images, each accompanied by five human-generated captions.  
The preprocessing steps for captions include:  
- Converting text to lowercase.
- Removing special characters and numbers.
- Eliminating extra spaces.
- Discarding single-character words.
- Adding 'startseq' and 'endseq' tags to mark the beginning and end of each caption.  

The VGG16 model extracts high-level visual features from the images, while the tokenized caption data is used as input for the LSTM model.

## Evaluation
The model’s performance is assessed using BLEU-1 and BLEU-2 scores, which measure the precision of n-grams between generated and reference captions.  
- **BLEU-1**: Measures **unigram (single word) precision**, indicating how accurately the model captures relevant keywords.  
- **BLEU-2**: Measures **bigram (two-word pairs) precision**, reflecting the fluency and coherence of generated captions.

### Results:
- **BLEU-1 Score**: 56.40% – indicating excellent keyword accuracy.  
- **BLEU-2 Score**: 34.29% – reflecting good fluency and the correct use of word pairs.  

## Conclusion
This project demonstrates the use of deep learning models to generate meaningful captions for images. The combination of VGG16 and LSTM delivers promising results, with BLEU scores indicating that the generated captions align well with human descriptions.
