# Kaggle SSH
Connect to Kaggle using SSH

# Prerequisites
1) You must have a Ngrok authentication token. Signing up for Ngrok is free and can be done in a couple minutes using a throwaway email

# Getting Started
1) Open a new kaggle notebook and navigate to: File -> Import Notebook -> Github
2) Paste the following link then click "Import": https://github.com/slooi/kaggle-ssh/blob/main/Kaggle_SSH.ipynb
3) Add your Ngrok token to `NGROK_AUTH_TOKEN` defined at the top of the `Kaggle_SSH.ipynb` file
4) (Optional) Change the username `USER_NAME` and password `USER_PASSWORD` for your kaggle environment
5) Click the "Run All" button to run the entire file
6) After the file has finished running, a ssh command should appear at the very bottom of the 2nd code cell along with the your password `USER_PASSWORD`. Execute the ssh command in your local terminal
7) Type in your password when your local termal prompts you
8) DONE!
