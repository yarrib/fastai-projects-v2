# fish classifier with fast.ai

The contents of this repo include 3 notebooks that train a fish classifier on images of various US and India fish obtained through the bing image api (from Azure)

Please ignore the Procfile, the runtime.txt, and requirements_heroku.txt files. Those are files used when the heroku deployment was being tested (a failure!).

## Instructions to run on your machine (windows, though running on linux/macos are pretty similar)

1) Download the repo and unzip it (or clone it if you have the github cli on your machine)

  ![image](https://user-images.githubusercontent.com/54746480/164243256-5c976004-949a-40d1-a3eb-49c23bfee144.png)

  + <i> (github cli) gh repo clone yarrib/fish-classifier-innov95 </i>


2) using your choice of terminal, create the virtual environment

  + this assumes you have python 3.9.x or later. please install python first by downloading from [python docs](https://www.python.org/downloads/?msclkid=d6a84840c0af11ecb8ac528392b60399)

  ![image](https://user-images.githubusercontent.com/54746480/164244856-6a49c476-ea2b-4c6e-90ed-0cd7c6264fec.png)
  

3)  install packages from the requirements.txt file

  + activate the environment first:
  
      - windows: <i> (powershell) ./[env_name]/Scripts/activate </i>
      - mac/linux: <i> (bash/zsh) source ./[env_name]/bin/activate </i>


  + install from requirements:

  ![image](https://user-images.githubusercontent.com/54746480/164245713-74e8bf8e-831b-4591-9fe6-e1261bb59103.png)

4) run the files in jupyter (if you want to experiment). assumes you are in the same directory as the notebook files. you won't be able to successfully run any of the notebooks besides the <i>notebookwebapp.ipynb</i> because of the api key and image dependencies (plus no gpu support most likely) not in this repo

  + <i> (powershell) jupyter notebook </i> (will open in browser window)

4b) run the webapp in voila:

  + this can take a while the first time, because it will pull the ~85mb trained model file called <b>model.pkl</b> from my google drive
  + <i> (powershell) voila notebookapp.ipynb </i>


...and thats it!

