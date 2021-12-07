# The is a Makefile
# Primarily used for Continuous Integration CI
# This is a good starting point for the project and often will evolve as more automation is needed



# This step sets up python virtual environment for the project
env:
	python -m venv env && \
		source env/bin/activate

# This step installs software via the make install command
install:
	pip install --upgrade pip &&\
		pip install -r requirements.txt

# This step checks the syntax errors via the make lint command
lint:
	pylint --disable=R,C hello.py

# This step runs tests via the make test command
test:
	python -m pytest -vv test_hello.py
