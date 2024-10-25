# EMOTION DETECTION FROM BENGALI TEXT BASED ON WORD SENSE DISAMBIGUATION 

## Introduction
Word sense disambiguation is concerned with accurately determining the sense of a polysemous word within a given text based on its contextual usage. For instance, Bengali words like মাথা (Māthā - head), হাত (Hāta - hand/arm), কড়া (Kaṛā - hard), গুল (Gula -rose), মুখ (Mukha - face), বাদ (Bāda - without), বড় (Baṛa - big), and সারা (Sārā - whole) exhibit different meanings depending on their context. Detecting the correct sense of such polysemous words is a challenging task and is central to WSD research. A WSD system aims to automatically identify the correct sense of polysemous words using machines, thereby resolving meaning-level ambiguities.

## Objective
Our primary objective is to develop a system that can detect the correct emotion (classified as positive, negative, or neutral) conveyed by a Bengali paragraph containing polysemous words based on their correct sense. 
The work presented in this project aims to provide comprehensive insights into the effectiveness of supervised learning methods for WSD in sentiment analysis of Bengali text.
The experimental results aim to meet the project's objectives and provide a path for expanding knowledge in this domain by improving existing research. 

## Contents
* Dataset.zip - It contains the whole dataset that we create and use. Initially, 30 polysemous words with at least 3 distinct senses are selected. Each sense has been associated with 3 distinct emotions (Positive, Negative, Neutral respectively). 30 paragraphs with respect to each sense corresponding to the 3 particular emotions have been collected for each of the 10 selected polysemous words. Estimated size of dataset: 30 𝑤𝑜𝑟𝑑𝑠× 3 𝑠𝑒𝑛𝑠𝑒𝑠×30 𝑝𝑎𝑟𝑎𝑔𝑟𝑎𝑝ℎ𝑠 𝑓𝑜𝑟 𝑒𝑎𝑐ℎ 𝑒𝑚𝑜𝑡𝑖𝑜𝑛=2700 paragraphs in total for the entire set.
* codes.zip - In contains the four codes (.ipynb), numbering them with an underscore at the end of their name. It also contains all csv files of all text files.

## Conclusion
The work represents a new dataset consisting of 30 polysemy words, where each word carries three distinct senses associated with three distinct emotions (positive, negative, neutral) and each sense consists of 30 distinct paragraphs, which can be also used in future in any work with Bengali polysemy words. 
We suggest a method where we look not only at the sentence with the target word but also the sentences before and after it. This helps us understand the emotions better in a paragraph and improves the accuracy of our emotion detection system. Then, in the feature extraction stage, we create the 𝑚 × 𝑛 matrix, where 𝑚 represents the number of documents and n number of unique features. Now, in the next step, it trains the obtained features for 4 different classifiers; these are ID3, CART, NB, and MLP, SVM. It achieves 74.01%, 74.31%, 80.69%, 82.59%, and 66.19% accuracy, respectively. Finally, we trained it with our proposed classification model, BEN-RS-ANN (that is generated for the classification of Bengali emotion on polysemy words) and even applied our heuristic method to determine the number of hidden neurons and got an improvement to 81.29% accuracy overall. In that case, the proposed classification model provides more accuracy than the previously mentioned well known models.
