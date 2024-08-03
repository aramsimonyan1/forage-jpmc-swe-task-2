# J.P. Morgan Chase software engineering program. Task 2

## Starter repo and setting up dev environment
###
    Fork and clone the repo for task 2 of JPMC's Forage program: https://github.com/theforage/forage-jpmc-swe-task-2
    Remember to uncheck the “Copy the main branch only” box in the fork dialog on GitHub. 
    A model answer has been provided in a separate branch from main.

    Create a new virtual environment in the project root. e.g. by using the venv module in Python:
    $python -m venv venv 
    This will create a new directory named venv in your project root, containing the virtual environment.

    Activate the Virtual Environment (windows  /  linux):
    $.\venv\Scripts\activate     /     $source venv/bin/activate

    Install all project dependencies. These are listed in the requirements.txt file:
    $pip install -r datafeed/requirements.txt

    Use npm, to install a series of javascript dependencies to your machine. If you already have access to npm on your system, you can skip this step. Otherwise, follow the instructions here (npm comes bundled with nodejs): https://nodejs.dev/en/learn/how-to-install-nodejs/
    For this project to work, you must have node 18.10.0 installed on your machine. Ensure you have the correct version by running “node -v” in your terminal. If you do not, consider using nvm to install the correct version for you.

    Install the necessary dependencies by running `npm install` from the project repo
    $npm install


## The objective (already completed)
Fix the client-side web application so that it displays a continuously updating line graph (whose y-axis is the stock’s top_ask_price and the x-axis is the timestamp of the stock) as it gets data from the server application. Currently, the web application only gets data every time you click on the 'Start Streaming Data' button and does not aggregate duplicated data.


## To run 
###
    First, start the python server from the root of the project repo:
    $python datafeed/server3.py

    Next, open a new terminal and start the client by running:
    $npm start

    If your browser didn't pop up, navigate to the below url and cick 'Start Streaming Data':
    http://localhost:3000/
