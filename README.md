# README

The purpose of this repo is to have a quick and easy place to go and grab the Kaggle file structure to get started on competitions, using the setup that I prefer on my local machine.

Kaggle has a specific file structure that it recommends be used locally, to make it easier to upload notebooks and code to its cloud-based system, called Kaggle Scripts.

In order to familiarize myself with the directory structure that Kaggle prefers, I created this repo and added it to Github. While there are plenty of bits of code from Kaggle's 2015 West Nile Virus competition posted on Github, none of them are organized using the structure that Kaggle's new online notebook format advocates. You can read more about this below, which even includes a link to download your own copy of the file structure.

**Please note that Kaggle has specific rules against sharing of competition data, and this repository attempts to abide by those rules.** If you end up forking this repo and using git to save your competition script file changes, but git doesn't see your file, you may want to check the `.gitignore` file to be certain it is configured to suit your purposes.



****
### ORIGINAL README FROM KAGGLE BELOW
****

*Please note that some elements (such as info about **R**) have been removed or modified.*

[Kaggle Scripts](https://www.kaggle.com/c/predict-west-nile-virus/scripts) are a great way to share models, visualizations, or analyses with other Kagglers.

You can run scripts right on Kaggle without ever downloading the data, but for iterating on your script, you'll probably find it's easier to work locally (and then copy your script to Kaggle for sharing).

## Directory Structure

It helps to set up the same directory structure that we have running on Kaggle. (Then you don't have to change any paths when copying the script to Kaggle.) [This file](https://www.kaggle.com/c/predict-west-nile-virus/download/west_nile.zip) sets up the directory structure (including all of the competition data):

- `input`: this contains all of the data files for the competition
- `working`: on Kaggle, scripts run with this as the working directory. We recommend you do the same thing locally to avoid mixing output files with source files.
- `src`: Source scripts. We've provided some examples to get you started.

## Python3 Environment

We have Github repositories showing how our ~~[R](https://github.com/Kaggle/docker-r) and~~ [Python](https://github.com/Kaggle/docker-python) environments are set up. We plan to make it very easy to work with the exact same environment locally, but at this point it may be easier to work with whatever environment you already have. (If you use Python or R packages locally that turn out to be missing in our online environment, we can probably add them for you.)


Do make sure you're using **Python 3**, though.

For example, run this command to activate your Python 3 environment (assuming you have one already created named `py35`):

   ```source activate py35```



## Command Line Execution

In your shell, you can navigate to the `working` directory, and run a script by saying:

`python ../src/measurement_locations.py`

Then open `working/output.html` to view the results!
