# {{cookiecutter.project_name}}

<p align="center">
  <a href="" rel="noopener">
 <img width=200px height=200px src="https://i.imgur.com/6wj0hh6.jpg" alt="Project logo"></a>
</p>

<h3 align="center">{{cookiecutter.project_name}}</h3>

<div align="center">

  [![code coverage](coverage.svg "Code coverage")]()
</div>

---


## 🧐 About <a name = "about"></a>
{{cookiecutter.project_short_description}}

## 🔖 Project structure

```
{{cookiecutter.project_name}}/
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
|    |- util/           # Script to store a utility method used in this project
|    |- visualization/  # Script to create exploratory and results oriented visualiazations
|- tests/               # Test files should mirror the src folder
```

## 🏁 Getting Started <a name = "getting_started"></a>
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Clone the project
```
git clone {{cookiecutter.gitlab_repo_url}}
```

### Install dependencies
Setup your environement and install project dependencies
```
make requirements
```

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
{{cookiecutter.full_name}} - {{cookiecutter.email}}