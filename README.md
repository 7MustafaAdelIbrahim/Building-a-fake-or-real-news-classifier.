## Building-a-fake-real-news-classifier.
      Identify and classify fake news articles.
---
<h1 style="text-align: center;font-size: 30px; color: #013b86;">Fake or Real. Two sides of the same coin</h1>
<center><img style="width: 600px;" src="https://images.ctfassets.net/yqezig6gzu6c/5ur280lovm0DKoHmlEGe1P/9779c9555ebed3dbd7e3445d0a666843/https___cdn2.hubspot.net_hubfs_656775_Fact_20Fake_201200_20x_20627px_2x-100_20copy.jpg?w=900&q=100"></center>


From my point of view, what we're in need most these days is a classifier to differentiate between true and fake news. False and misleading news has increased a lot in recent times, especially on social media platforms. Hence the inspiration to work on building a machine learning model to classify fake news.

Then came the fake news which spread across people as fast as the real news could. Fake news is a piece of incorporated or falsified information often aimed at misleading people to a wrong path or damage a person or an entity’s reputation.

### About our dataset.
[Our dataset from kaggle] (https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset) contains two datasets, one is for real news, and the other is not.
### What i have done....
After importing our two datasets, we have 23481 entries in fake news datasets, and 21417 entries in real ones, and we do not have any missingness.
##### Data Cleaning
Identification and removal of errors if any in the gathered information. This process is carried out mainly to improve the dataset’s quality, make it reliable, and provide accurate decision-making processes.
#### Text pre-processing
      We need to perform two steps to make this dataset suitable for machine learning.
Our target is to standardize the text. We'll be covering the common ones. This involves steps like converting words to lowercase, removing unnecessary whitespace, removing punctuation, removing commonly occurring words or stopwords, expanding contracted words like don't and removing special characters such as numbers and emojis, and getting the base form of words. For instance, 'Reduction' gets converted to its base form, which is reduce.
##### Remove english stopwords.
There are some words in the English language that occur so commonly and does not contain any useful information. So, it's often a good idea to ignore them, as they could skew our analysis and may negatively affect the machine learning model performance. Examples include articles such as a and the, be verbs such as am, is and are and pronouns such as he and she.
##### Data Exploration/Analysis:
Various visualization techniques are carried out here to understand the dataset in terms of its characteristics namely, size, quantity, etc. This process is essential to better understand the nature of the dataset and get insights faster.
![fake vs real](https://user-images.githubusercontent.com/84151016/180622770-8ab4e67e-b158-4652-9ca1-0241359d9b98.png)

#### Some feature engineering.
<p>
<img src= "https://user-images.githubusercontent.com/84151016/180622788-956cad21-4969-4f35-aa01-b3cbadc2d627.png", width=450, height=400>
<img src= "https://user-images.githubusercontent.com/84151016/180622808-5c7cbf9d-9579-4fb1-baed-c3df062f0254.png", width=450, height=400>
</p>

#### Bag of words.

![bag of words](https://user-images.githubusercontent.com/84151016/180622802-bd250e2c-c9d0-40b6-8df1-9306824ff5e1.png)


##### Data Modelling

### Model evalution.
            A confusion matrix gives a useful breakdown of predictions versus known values. It has four cells which represent the counts of:

To further evaluate our model, we can check the confusion matrix which shows correct and incorrect predicted labels. It's a bit easier to read, as the first value and last value of the matrix, or the main diagonal of the matrix show true scores, which means the true classification of both Real of fake news. In a confusion matrix, the predicted labels are shown across the top and the true labels are shown down the side.

![download](https://user-images.githubusercontent.com/84151016/158228346-91af4ee0-0b68-41be-975c-39db678085cf.jpg)

In addition to accurcy metric, there are two other useful metrics:

Precision, which is the proportion of positive predictions which are correct. For all flights which are predicted to be delayed, what proportion is actually delayed?
And recall, which is the proportion of positives outcomes which are correctly predicted. For all delayed flights, what proportion is correctly predicted by the model?
The precision and recall are generally formulated in terms of the positive target class. But it's also possible to calculate weighted versions of these metrics which look at both target classes.

