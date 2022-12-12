## CHATBOT FOR HEALTHCARE SYSTEM USING AI
*****************************************
Healthcare is very important to lead a good life. However, it is very difficult to obtain a
consultation with a doctor for every health problem. The idea is to create a medical chatbot
using Artificial Intelligence that can diagnose the disease and provide basic details about the
disease before consulting a doctor. This will help to reduce healthcare costs and improve
accessibility to medical knowledge through medical chatbots.



## Prerequisites
****************

=>Download and install python :
-------------------------------
  https://www.python.org/downloads/

=>Download and install Microsoft Visual Studio C++ :
----------------------------------------------------
  https://learn.microsoft.com/en-US/cpp/windows/latest-supported-vc-redist?view=msvc-170

=>Download and install conda :
------------------------------
  https://www.anaconda.com/products/distribution



=>Create an environment for installing rasa:
============================================

We use conda to create the virtual environment, open your preferred command line/terminal/shell in the extracted directory and all the commands are to be performed here.

Execute the code to create an env in the same directory <code> conda create --name env_name python==3.7.6 </code> 

Activate env by executing code <code> conda activate env_name </code>

=>Install all dependencies:
---------------------------

 =>install ujason
<code> conda install ujson </code>

 =>install Tensorflow
<code> conda install tensorflow </code>

 =>install rasa
<code> pip install rasa or pip3 install rasa </code>

 =>install flask
<code> pip install flask or pip3 install flask </code>

 =>install requests
<code> pip install requests or pip3 install requests </code>


## STEPS TO BE FOLLOWED TO RUN THE CHATBOT:
*******************************************

Download and extract the zip file

Now open a terminal(Terminal-1):
================================

Activate env by executing: <code> conda activate env_name </code>

Go to rasabot directory: <code> cd rasabot </code>

Train the model: <code> rasa train </code>

If successfully trained prompt returns: "Your Rasa model is trained and saved"

Run the following command to start rasa server: <code> rasa run -m models --endpoints endpoints.yml --port 5002 --credentials credentials.yml </code>

Prompt returns: Rasa server is up and running.


Now open another Terminal (Terminal-2):
=======================================

Go to web_app directory: <code> cd web_app </code>

Run the following command to start flask server: <code> flask run </code>

Prompt returns: Running on http://127.0.0.1:5000 or may be something in the same format.

After sucessfully running rasa and flask server
  copy the url "http://127.0.0.1:5000" prompted on the terminal-2, paste it in any default browser and run it.



## Technologies used:
*********************

**Client:** HTML, CSS, Javascript

**Server:** Python Flask

**Chatbot framework:** Rasa



## Tool/IDE used:
*****************

**Visual Studio Code**

**Anaconda**


## Images:
*****************
![web_app_implementation(1)](https://user-images.githubusercontent.com/114933781/207016061-d7502857-3ef2-4be3-965f-305f9b9bdac7.png)
![web_app_implementation(2)](https://user-images.githubusercontent.com/114933781/207016352-ff97e606-64d7-4329-9514-9b4f26de88b2.png)

