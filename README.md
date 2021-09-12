# ml-svm-spamassassin-spam-classifier
This jupyter notebook application fits a Support Vector Machine model to classify emails as spam or not using the [SpamAssassin Public Corpus](https://spamassassin.apache.org/old/publiccorpus/) data, and also provides the ability to predict new emails.

---

## Setup
 - Clone this repo to your desktop.
 - Extract the data.rar file to the root directory of this project.
 - cd to the root directory and create a virtual enviornment (recommended).
 - Run `pip install -r requirements.txt` to install all the dependencies.
 - Run `jupyter notebook` to open up the notebook in your browser.

## Usage
To predict new emails:
  - Run all cells in the jupyter notebook to train the model.
  - Add the txt file(s) of the new raw sample(s) you want to predict to the "data\samples" directory. (Note: Make sure the data.rar file has already been extracted.)
  - Run `predictSamples(filenames)` where "filenames" is a python list of the names of all the samples you want to predict, e.g., `filenames = ['emailSample1.txt', 'emailSample2.txt']`.
