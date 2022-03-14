# Building-a-fake-real-news-classifier.
      Identify and classify fake news articles.
---
<h1 style="text-align: center;font-size: 30px; color: #013b86;">Fake or Real. Two sides of the same coin?</h1>
<center><img style="width: 700px;" src="https://images.ctfassets.net/yqezig6gzu6c/5ur280lovm0DKoHmlEGe1P/9779c9555ebed3dbd7e3445d0a666843/https___cdn2.hubspot.net_hubfs_656775_Fact_20Fake_201200_20x_20627px_2x-100_20copy.jpg?w=900&q=100"></center>


Model evalution.
Confusion matrix
To further evaluate our model, we can check the confusion matrix which shows correct and incorrect predicted labels. It's a bit easier to read, as the first value and last value of the matrix, or the main diagonal of the matrix show true scores, which means the true classification of both Real of fake news. In a confusion matrix, the predicted labels are shown across the top and the true labels are shown down the side.

A confusion matrix gives a useful breakdown of predictions versus known values. It has four cells which represent the counts of:

![download](https://user-images.githubusercontent.com/84151016/158228346-91af4ee0-0b68-41be-975c-39db678085cf.jpg)


True Negatives (TN) — model predicts negative outcome & known outcome is negative

True Positives (TP) — model predicts positive outcome & known outcome is positive

False Negatives (FN) — model predicts negative outcome but known outcome is positive

False Positives (FP) — model predicts positive outcome but known outcome is negative.
