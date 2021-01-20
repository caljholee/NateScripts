# NateScripts

#MassImageLabeller

MassImageLabeller is a Python script that automates the labelling of images, and outputs a .csv file that has an index of path file names, and a column name of Name 1 - Name 10 and Score 1 - Score 10. Name 1 is the most likely label, Name 10 is the least likely label, Score 1 is the corresponding score to name 1 (how accurate the label is), and score 10 is the corresponding score to name 10. 

#Installation
1) Follow instructions on https://cloud.google.com/vision/docs/quickstart-client-libraries#install_the_client_library from Steps (1-4) Put JSON file containing key on desktop. 
2) Follow instructions on https://cloud.google.com/sdk/docs/install (Steps 1, 2a, 2c) *this is based on the fact that Python and Pandas is already installed. If python not installed (Python Development Environment Setup Guide), if pandas not installed (https://pandas.pydata.org/pandas-docs/stable/getting_started/install.html) 
3) Install Client Library https://cloud.google.com/vision/docs/quickstart-client-libraries#install_the_client_library (pip install --upgrade google-cloud-vision)

#Usage 
*On Line 8: replace 'Nate-e5be74c2cdea.json' to the path of the JSON file that contains your service account key. **If current directory of script is desktop, you should be able to just replace 'Nate-e5be74c2cdea.json' with name of the new JSON file. 
1) Create a folder in desktop, and input images that you want to label within that folder. Give Folder a Name (i.e. ‘Image_Set’)
2) In the python file, after line 36 replace “Images” in a = mass_label("Images") with name of folder i.e. ‘Image_Set’
3) If you’d like to name the csv file differently or put it in a different location, modify the path ‘/Users/bots/Desktop/‘ in a.to_csv(r'/Users/bots/Desktop/converted.csv') to the desired location and if you’d like to modify the name of the file, change ‘converted.csv’ to ‘name.csv’ 

#For any questions: jholee@berkeley.edu or 9496898276

