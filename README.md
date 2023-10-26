# Kaggle SSH
Connect to Kaggle using SSH

# Prerequisites
1) You must have a Ngrok authentication token. You receive one when signing up for Ngrok. Signing up is free and can be done in a couple minutes using a throwaway email

# Getting Started
1) Open a new kaggle notebook and navigate to: File -> Import Notebook -> Github. A field accepting URLs should appear
2) Paste the link https://github.com/slooi/kaggle-ssh/blob/main/Kaggle_SSH.ipynb into the field then click "Import": 
3) Add your Ngrok token to `NGROK_AUTH_TOKEN` defined at the top of the `Kaggle_SSH.ipynb` file
4) Change the username `USER_NAME` and password `USER_PASSWORD` for your kaggle environment to something more secure
5) Click the "Run All" button to run the entire file
6) After the file has finished running, a ssh command and your password should appear at the very bottom of the 2nd code cell. Execute the ssh command in your local terminal
7) Type in your password when your local termal prompts you
8) DONE!
