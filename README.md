# XAIandDataPrivacy

This repository includes the experiments of the bachlor's thesis "Quantitive Evaluation of the Expected Antagonism of Explainability and Privacy".
I show that the [scikit-learn](https://scikit-learn.org/) implementation of [Individual Conditional Expectation](https://www.tandfonline.com/doi/full/10.1080/10618600.2014.907095) can enable the privacy attacks membership inference and training data extraction. Additionaly, counterfactuals from the explainer [DiCE](https://github.com/interpretml/DiCE) are shown to enable training data extraction if the method `kd-tree` is used.
The experiments use the datasets ["Adult Data Set" by UCI](https://archive.ics.uci.edu/ml/datasets/Adult) and ["Logistic regression To predict heart disease" from Kaggle](https://www.kaggle.com/dileep070/heart-disease-prediction-using-logistic-regression).

## Execute with Docker

Run command `docker build -t xaidataprivacy .` in the directory with the Dockerfile.

Then you can run the image mounted to your working directory with the following command: `docker run -p 8888:8888 -v WORKING_DIRECTORY:/home/jovyan/work xaidataprivacy`.
The working directory should be the directory of this repository.

Open the jupyter notebook at the URL specified in the command prompt.