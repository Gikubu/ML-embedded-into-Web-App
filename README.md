Description
In this project, I create a machine learning model from the sepsis dataset. Also, I will create an API that will integrate the ML model using FastAPI. The App will interact with the model to classify the sepsis illness. Finally, I will containerize my application with a docker.

python MIT licensed Python

Code	Name	Published Article	Deployed App
P 6	Embedding ML model into web application	Medium
LinkedIn	
Note on Data
This is a summary of the information contained in the data
ID: number to represent patient ID
PRG: Plasma glucose
PL: Blood Work Result-1 (mu U/ml)
PR: Blood Pressure (mm Hg)
SK: Blood Work Result-2 (mm)
TS: Blood Work Result-3 (mu U/ml)
M11: Body mass index (weight in kg/(height in m)^2)
BD2: Blood Work Result-4 (mu U/ml)
Age: patients age (years)
Insurance: If a patient holds a valid insurance card. 0: Patient without insurance, and 1: Patient with insurance
Sepsis: Positive: if a patient in ICU will develop a sepsis , and Negative: otherwis

Screenshot of Deployed App
Setup
Install the required packages to be able to run the evaluation locally.

You need to have Python3 on your system. Then you can clone this repo and being at the repo's root (root :: repo_name> ...) follow the steps below:

Windows:

  python -m venv venv; venv\Scripts\activate; python -m pip install -q --upgrade pip; python -m pip install -qr requirements.txt  
Linux & MacOs:

  python3 -m venv venv; source venv/bin/activate; python -m pip install -q --upgrade pip; python -m pip install -qr requirements.txt  
The both long command-lines have a same structure, they pipe multiple commands using the symbol ; but you may manually execute them one after another.

Create the Python's virtual environment that isolates the required libraries of the project to avoid conflicts;
Activate the Python's virtual environment so that the Python kernel & libraries will be those of the isolated environment;
Upgrade Pip, the installed libraries/packages manager to have the up-to-date version that will work correctly;
Install the required libraries/packages listed in the requirements.txt file so that it will be allow to import them into the python's scripts and notebooks without any issue.
NB: For MacOs users, please install Xcode if you have an issue.

Run FastAPI
Run the demo apps (being at the repository root):

FastAPI:

Demo

uvicorn src.demo_01.api:app --reload 
Go to your browser at the following address, to explore the api's documentation :

http://127.0.0.1:8000/docs

Resources
Here are some ressources you would read to have a good understanding of FastAPI :

Tutorial - User Guide
Video - Building a Machine Learning API in 15 Minutes
FastAPI for Machine Learning: Live coding an ML web application
Video - Deploy ML models with FastAPI, Docker, and Heroku
FastAPI Tutorial Series
Http status codes
Author
Joseph Gikubu