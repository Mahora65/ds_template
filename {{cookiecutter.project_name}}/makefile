## Install dependencies
.PHONY: requirements
requirements:
	python3 -m pip install --upgrade pip
	python3 -m pip install pip-tools
	python3 -m piptools compile --upgrade --output-file requirements.txt requirements.in
	python3 -m piptools compile --upgrade --output-file requirements-dev.txt requirements-dev.in
	python3 -m piptools sync requirements.txt requirements-dev.txt
## Run all pre-commit hooks
.PHONY: precommit
precommit:
	pre-commit run --all-file --show-diff-on-failure
## Lint your code using pylint
.PHONY: lint
lint:
	python3 -m pylint --version
	find . -type f -name "*.py" | xargs python3 -m pylint
## Run tests using pytest
.PHONY: tests
test:
	python3 -m pytest --version
	python3 -m pytest tests
## Format your code using black
.PHONY: black
black:
	python3 -m black --version
	python3 -m black .
## autogenerate documentation using pdoc
.PHONY: docs
docs:
	python3 -m pdoc --version
	python3 -m pdoc --html --output-dir docs src
