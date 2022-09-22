# ML-for-Texts
Project Description<br>
The Film Junky Union, a new edgy community for classic movie enthusiasts, is developing a system for filtering and categorizing movie reviews. The goal is to train a model to automatically detect negative reviews. You'll be using a dataset of IMBD movie reviews with polarity labelling to build a model for classifying positive and negative reviews. It will need to reach an F1 score of at least 0.85.
Project Instructions<br>
Load the data.<br>
Preprocess the data, if required.<br>
Conduct an EDA and make your conclusion on the class imbalance.<br>
Preprocess the data for modeling.<br>
Train at least three different models for the given train dataset.<br>
Test the models for the given test dataset.<br>
Compose a few of your own reviews and classify them with all the models.<br>
Check for differences between the testing results of models in the above two points. Try to explain them.<br>
Present your findings.<br>
Important! The project template already contains some code snippets for your convenience, so you can use them if you'd like. If you want to start right away from a clean sheet, just remove all those code snippets. Here's the list of code snippets:<br>
A bit of EDA with some plots<br>
evaluate_model()<br>
a routine to evaluate a classification model which conforms to the scikit-learn predict interface<br>
BERT_text_to_embeddings()<br>
a routing to convert a list of texts into embedding with BERT<br>
The main job to build and evaluate models is your own.<br>
As you can see from the project template, we suggest trying classification models based on logistic regression and gradient boosting, but feel free to try other methods. You can mess around with the project template's structure as long as the project's instructions are completed.<br>
You don't have to use BERT for the project because it is very demanding for computational power and will be very slow on the CPU for the complete dataset. Because of this, BERT usually needs to be executed on GPU for adequate performance. However, you are more than welcome to try and include BERT in the project for a part of the dataset. If you want to do this, we suggest doing so locally and only taking a couple hundred of objects per each part of the (train/test) dataset to avoid waiting too long. Make sure to indicate your use of BERT in the first cell (the header of your project).<br>
Data Description<br>
The data is stored in the imdb_reviews.tsv file. Download the dataset.<br>
The data was provided by Andrew L. Maas, Raymond E. Daly, Peter T. Pham, Dan Huang, Andrew Y. Ng, and Christopher Potts. (2011). Learning Word Vectors for Sentiment Analysis. The 49th Annual Meeting of the Association for Computational Linguistics (ACL 2011).<br>
Here's the description of the selected fields:<br>
review: the review text<br>
pos: the target, '0' for negative and '1' for positive<br>
ds_part: 'train'/'test' for the train/test part of dataset, correspondingly<br>
There are other fields in the dataset. Feel free to explore them if you'd like.<br>
