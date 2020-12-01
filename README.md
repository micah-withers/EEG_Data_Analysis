EEG Data Analysis
===

Analyzing EEG data to determine which group, Alcoholic or Control, the subject belongs to using classification models.
---

**Requirements**
* EEG dataset from Kaggle (the data is not mine)
* Anaconda
* Python >=3.6
* Pandas
* Sci-kit Learn

**Installation**  
Open terminal or an Anaconda Prompt  

Create an environment with Python 3.6 or later:  
>$ conda create --name myenv python  
_Replace "myenv" with the environment name of your choice_  

Activate the new environment:  
>$ conda activate myenv  

Install Pandas:  
>_With conda:_  
$ conda install -c conda-forge pandas  
_With pip:_  
$ pip install -U pandas  

Install Sci-kit learn:  
>_With conda:_  
$ conda install -c conda-forge scikit-learn 
_With pip:_  
$ pip install -U scikit-learn 

Clone this repository and download [dataset](https://www.kaggle.com/nnair25/Alcoholics)
>Inside the repository, create a "data" folder
>Download the whole dataset from the link above and extract the contents into the folder you just created

**Usage**
>All code is executable. Models were created to classify based on different columns, but there could be other ways of classfiying each trial.
One file uses logistic regression and the other a neural net (ends in "nn"). 

**NOTE:** these models are not perfect because of the varying values for each sample column. 
Transforming the data before testing it would normalize all of the sensor values for each sample
and lead to inaccurate results. 
