# Simple project

## Data

Download data from UCI and unzip:
```bash
$ wget https://archive.ics.uci.edu/ml/machine-learning-databases/00240/UCI%20HAR%20Dataset.zip
$ unzip "UCI HAR Dataset.zip"
```
Make sure that data looks like this:
```bash
$ ls -l UCI\ HAR\ Dataset
total 64
-rw-r-----  1 dima  staff   6304 Feb 15  2015 README.txt
-rwxr-xr-x  1 dima  staff     80 Oct 10  2012 activity_labels.txt
-rwxr-xr-x  1 dima  staff  15785 Oct 11  2012 features.txt
-rwxr-xr-x  1 dima  staff   2809 Oct 15  2012 features_info.txt
drwxr-xr-x  6 dima  staff    204 Nov 29  2012 test
drwxr-xr-x  6 dima  staff    204 Nov 29  2012 train
```

## Running scripts

- Experiment 1

  This script is just the same code we had in the notebook.
```bash
$ python simple_experiment.py
```
- Experiment 2

  This script uses arparse to define the model to run.
```bash
$ python simple_experiment2.py --model-type logistic
```
- Experiment 3

  This script uses a simple YAML config file to define the model to run.
```bash
$ python simple_experiment3.py ./config.yaml
```
- Experiment 4

  This script demonstrates how to use more complex YAML files.
```bash
$ python simple_experiment4.py ./config2.yaml
```

