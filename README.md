# SketchSense

The code within this repository is designed to meticulously collect and preprocess the drawing data. Furthermore, it employs sophisticated algorithms to extract a comprehensive set of parameters including height, width, roundness, elongation, and complexity. These refined features are then channeled into a K-Nearest Neighbors (KNN) model, facilitating accurate predictions of the drawings drawn by the user.

# About Project

This project is divided in two parts:
  1. Drawings Collection (data collection)
  2. Prediction of drawings drawn by the user.

For the first part of the project, creator.html file is created. This webpage allows user to contribute to dataset. Below is the step wise explainattion as how it is working:
  1. whenever user will be on https://sketch-sense-pulakpj9s-projects.vercel.app/web/creator.html page, he/she would be able to see page where he/she would be asked to enter their name.
  2. As soon as one would enter name and click next he/she would be asked to draw sketches of each of the 8 classes (car, fish, tree, bicycle, house, pencil, guitar, clock).
  3. After drawing the last sketch, user would see a thank you page and a json file containing information of each of the 8 sketches would get downloaded to his/her pc. 

For the second part of the project, viewer.html file is created. This webpage allows user to play with the site where user can draw any sketch of any of 8 cases and the website would try to predict the sketch. Below is the step wise explainattion as how it is working:
  1. whenever user will be on https://sketch-sense-pulakpj9s-projects.vercel.app/web/viewer.html page, he/she would be able to see page where he/she would be able to see whole dataset training as well as testing.
  2. On scrolling the page, also user can see the testing results of the model like in which type of sketches the model is able to predict what. This would help user to more closely uderstand the model.
  3. Also, A confusion matrix is plotted in right side of the screen which helps to evaluate the model and analysis the mistakes done by model more accurately.
  4. also, 2 buttons on the top right corner of the page code be seen.
  5. in that toggle input button, toggles the canvas where a user can draw his sketch. while toggle output button toggles the confussion matrix.

# How to run the code

1. Download the zip or clone this repo on your local machine.
2. Then open node folder in your terminal and run "npm install" command ( This will install all the dependencies and also will automatically run data generator , feature extractor and run evaluation scripts).
3. The previous step may take 10 - 15 minutes depending on one's local machine speed.
4. And at last go to web folder and open (viewer.html/ creator.html) file and run live server on it .
