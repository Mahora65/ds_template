# template_ds_project

<p align="center">
  <a href="" rel="noopener">
 <img width=200px height=200px src="https://i.imgur.com/6wj0hh6.jpg" alt="Project logo"></a>
</p>

<h3 align="center">Project Title</h3>

<div align="center">

  [![code coverage](coverage.svg "Code coverage")]()
</div>

---


## 🧐 About <a name = "about"></a>
Write about 1-2 paragraphs describing the purpose of your project.

## 🔖 Project structure

```
Project_folder/
|- bin/                 # Contains scripts and main files that should be run
|- config/              # Config files
|- data/
|    |- external        # Data from third party sources
|    |- interim         # Intermediate data that has been transform
|    |- processed       # The final, canonical data set for modeling
|    |- raw             # The original, immutable data dump
|- docs/                # Data dictionaries, manuals, and all other explanatory materieals
|- makefile             # Automatize task through make utility
|- models/              # Trained and serialized models, model predictions, or model summaries
|- notebooks/           # Notebooks for EDA and exploration
|- reports/             # Generated analysis as HTML, PDF, etc.
|    |- figures         # Generated graphics and figures to be used in reporting
|- secrets/             # Contains api keys and secret parameters. It should be ignored from git
|- src/                 # Source code - contains functions 
|    |- data/           # Script to download or generate data 
|    |- features/       # Script to turn raw data into features for modeling
|    |- models/         # Script to train models and then use trained models to make predictions
|    |- visualization/  # Script to create exploratory and results oriented visualiazations
|- tests/               # Test files should mirror the src folder
```

## 🏁 Getting Started <a name = "getting_started"></a>
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites
Setup your environement and install project dependencies
```
conda create -n my_project python=3.10
source activate my_project

python -m pip install pip-tools
pip-compile --output-file requirements.txt requirements.in requirements_dev.in
python -m pip install -r requirements.txt
```

### Installing

## 🔧 Running the tests
Tests are implemented in ./tests, you need to run the following command to run them.
```
make tests
```

## 🚀 Deployment
Add additional notes about how to deploy this on a live system.

## 🎈 Contributions
To contribute in this project, please setup locally the project following the steps  in Getting started section.
We use few packages to guarantee high quality code. Before commiting you can run:
To format you code using black
```
make black
```
To get warning message on non respect of pep8 code guidance:
(the command runs on all .py files in the project)
```
make lint
```
You can also run automatically, black, lint and few other packages to analyze and check your code base before commiting
```
make precommit
```

##  ✍️ Authors
