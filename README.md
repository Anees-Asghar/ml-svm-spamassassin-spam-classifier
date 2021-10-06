# ml-svm-spamassassin-spam-classifier
This jupyter notebook application fits a Support Vector Machine model to classify emails as spam or not using the [SpamAssassin Public Corpus](https://spamassassin.apache.org/old/publiccorpus/) data, and also provides the ability to predict new emails.

---

## Setup
- Clone this repo to your desktop.
- Extract the data.rar file to the root directory of this project.
- Create a new anaconda environment with all the requirements using the following command:

      conda env create -f environment.yml

- Activate the environment using (windows)

      activate spam-classifier-env

  or if you are on a linux machine

      source activate spam-classifier-env

- Run `jupyter notebook` from the root directory to open up the notebook in your browser.

## Usage

To predict new emails:
 - Run all cells in the jupyter notebook to train the model.
 - Add the txt file(s) of the new raw sample(s) you want to predict to the "data\samples" directory. (Note: Make sure the data.rar file has already been extracted.)
 - Run `predictSamples(filenames)` where "filenames" is a python list of the names of all the samples you want to predict, such as:
 
       filenames = ['emailSample1.txt', 'emailSample2.txt']
