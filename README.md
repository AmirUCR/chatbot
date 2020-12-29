# Brian Chatbot

You cannot clone and run this code without getting an authentication key from Google's API first. Acquire and place your service account information in a key.json file in the same directory as the .ipynb files before running this program. Unfortunately, I cannot give you a key. For the "Why?" see this https://www.youtube.com/watch?v=hrDcF-iwGhg


In case you are a new programmer, NEVER share your private key on GitHub or anywhere else. It happened to me, it was painful. Also this program will only talk back if you are on Windows. To make the talk-back functionality work with other OS, modify the last if-statement in the google_tts.ipynb file.

Before getting started, here is a demo https://www.youtube.com/watch?v=Nv-g-YnzYaA please note that this demo was recorded when I was using Amazon's Text-to-Speech API with the Brian voice. This repo contains code for Google's Text-to-Speech which sounds different, but provides the same functionality.

# What is This?

Brian is a simple but extensible Python-based chatbot that utilizes your computer's microphone in conjunction with Google Cloud Platform's Speech-to-Text API. It then references a dictionary of responses which correspond to your sentences and, using Google's Text-to-Speech API, talks the response back to you.

# How to Run This?
You need a Jupyter notebook/lab environment, Google Cloud Python library, and Wikipedia Python library


Follow this tutorial to install the required Google Cloud library and create a new private key https://cloud.google.com/text-to-speech/docs/libraries I also explain how to get a key below.


Log-in to your Google Cloud Console. Create a new project, name it anything you want. In the left panel, select APIs & Services, then Credentials. Under Service Accounts, click on Manage service accounts. + Create Service Account. Name it something descriptive, like chatbot. Under Keys, click ADD KEY, Create new key, type: JSON. Name the JSON file key.json and place it in the same directory as the .ipynb files that you download from this repo.

Cross your fingers and run chatbot.ipynb. If it doesn't work, feel free to create an Issue and we will figure it out together :)
