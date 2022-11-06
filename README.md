<h1>Project Description</h1>
The Film Junky Union, a new edgy community for classic movie enthusiasts, is developing a system for filtering and categorizing movie reviews. The goal is to train a model to automatically detect negative reviews. You'll be using a dataset of IMBD movie reviews with polarity labelling to build a model for classifying positive and negative reviews. It will need to reach an F1 score of at least 0.85.

<h2>Project Instructions</h2>
<ol><li>Load the data</li>
<li>Preprocess the data, if required</li>
<li>Conduct an EDA and make your conclusion on the class imbalance</li>
<li>Preprocess the data for modeling</li>
<li>Train at least three different models for the given train dataset</li>
<li>Test the models for the given test dataset</li>
<li>Compose a few of your own reviews and classify them with all the models</li>
<li>Check for differences between the testing results of models in the above two points. Try to explain them</li>
<li>Present your findings</ol></li>
Important! The project template already contains some code snippets for your convenience, so you can use them if you'd like. If you want to start right away from a clean sheet, just remove all those code snippets. Here's the list of code snippets:<br>

<ul><li>A bit of EDA with some plots</li>
<ul><li>evaluate_model()</ul></li>
<li>a routine to evaluate a classification model which conforms to the scikit-learn predict interface</li>
<ul><li>BERT_text_to_embeddings()</ul></li>
<li>a routing to convert a list of texts into embedding with BERT</ul></li>

The main job to build and evaluate models is your own.<br>
As you can see from the project template, we suggest trying classification models based on logistic regression and gradient boosting, but feel free to try other methods. You can mess around with the project template's structure as long as the project's instructions are completed.<br>

You don't have to use BERT for the project because it is very demanding for computational power and will be very slow on the CPU for the complete dataset. Because of this, BERT usually needs to be executed on GPU for adequate performance. However, you are more than welcome to try and include BERT in the project for a part of the dataset. If you want to do this, we suggest doing so locally and only taking a couple hundred of objects per each part of the (train/test) dataset to avoid waiting too long. Make sure to indicate your use of BERT in the first cell (the header of your project).<br>

<h4>Data Description</h4>
The data is stored in the imdb_reviews.tsv file. Download the dataset.<br>

<i>The data was provided by Andrew L. Maas, Raymond E. Daly, Peter T. Pham, Dan Huang, Andrew Y. Ng, and Christopher Potts. (2011). Learning Word Vectors for Sentiment Analysis. The 49th Annual Meeting of the Association for Computational Linguistics (ACL 2011).</i>

Here's the description of the selected fields:<br>
<ul><li>review: the review text</li>
<li>pos: the target, '0' for negative and '1' for positive</li>
<li>ds_part: 'train'/'test' for the train/test part of dataset, correspondingly</ul></li>

There are other fields in the dataset. Feel free to explore them if you'd like
