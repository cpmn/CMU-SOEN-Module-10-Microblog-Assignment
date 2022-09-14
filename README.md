# Installation Instructions

## Prerequisites 

_Provided are instructions for Mac OS X and Linux; if you're on Windows, we recommend you use the Windows Subsystem for Linux (WSL) and follow the Linux instructions._

1. If you don't have Python 3 installed already, follow the instructions below.  On all OS's, you can see if you have Python 3 installed by running `python3 --version`.  If you have Python 3 installed, you can skip to the next step.

* If you are using Linux or WSL in Windows, use the following [instructions](https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-programming-environment-on-an-ubuntu-20-04-server).  
* If you are on Mac OS X, first make sure you have [Xcode](https://developer.apple.com/xcode/) installed.  Next, install the Xcode command-line tools using the following command `xcode-select --install`.  Then, use the following [instructions](https://opensource.com/article/19/5/python-3-default-mac) on making Python 3 the default Python environment.

2. Install [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).

## Microblog

_All starter code for all of the assignments is available through Gradescope._

1. Create and activate a virtual environment for Python.  This should be run in your terminal.

```sh
python3 -m venv venv && source venv/bin/activate
```

2. Install the required Python dependencies.

```sh
pip3 install -r requirements.txt
```

3. Setup the database for the Flask service.

```sh
flask db upgrade && flask translate compile
```

4. Run the flask application.

```sh
python3 -m flask run
```

5. Verify you can access the application using your web browser by navigating to the microblog at: [http://127.0.0.1:5000/](http://127.0.0.1:5000/).

# Submission Instructions

1. Create an _assignment.txt_ file containing two lines.  The first line should be your GitHub ID, and the second line should be a link to your open pull request
2. Push your changes to your repo and go to the Gradescope assigment entitled Module 10: CI
3. Click the _Submit Assignment_ button (or _Resubmit Assignment_ button if you are submitting a second attempt)
4. Click the _Upload_ submission method
5. Select the _assignment.txt_ file from your local files
6. Click upload and wait for the results of the autograder
