# Kaggle SSH
Connect to Kaggle using SSH

# Prerequisites
1) You must have a Ngrok authentication token. You receive one when signing up for Ngrok. Signing up is free and can be done in a couple minutes using a throwaway email

# Getting Started
1) Open a new kaggle notebook and navigate to: File -> Import Notebook -> Github. A field accepting URLs should appear
2) Paste following link into the field:   https://github.com/slooi/kaggle-ssh/blob/main/Kaggle_SSH.ipynb
3) Then click "Import"
4) Add your Ngrok token to `NGROK_TOKEN` defined at the top of the `Kaggle_SSH.ipynb` file
5) Click the "Run All" button and wait until the final code cell has been executed
6) You will be prompted to run some code. Run it in your local terminal to ssh into your kaggle instance
7) DONE!
