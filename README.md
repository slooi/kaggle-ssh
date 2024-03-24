# Kaggle SSH
Connect to Kaggle using SSH

# Prerequisites
1) You must have a Ngrok authentication token. You receive one when signing up for Ngrok. Signing up is free and can be done in a couple minutes using a throwaway email

# Getting Started
1) Open a new kaggle notebook and navigate to: File -> Import Notebook -> Github. A field accepting URLs should appear
2) Paste following link into the field: <pre>https://github.com/slooi/kaggle-ssh/blob/main/Kaggle_SSH.ipynb
3) Then click "Import"
4) Add your Ngrok token to `NGROK_TOKEN` defined at the top of the `Kaggle_SSH.ipynb` file
5) Click the "Run All" button and wait until the final code cell has been executed
6) You will be prompted to run a script similar to the one provided below (however your script will have more lines). Run the script in your local terminal to ssh into your kaggle instance.
```
(
echo -----BEGIN OPENSSH PRIVATE KEY-----
echo b3BlbnNzaC1rZXktdjEAAAAABG5vbmUAAAAEbm9uZQAAAAAAAAABAAABlwAAAAdzc2gtcn
echo xLByZVU2oxzUgo02q4YpZ2gAkANXCCW4hr9pEH53R4aaPlLMsfPIQIaKMefEVT3VZ/v0u9
...... (YOUR SCRIPT WILL HAVE A BUNCH MORE LINES HERE. I HAVE SHORTENED THIS FOR BREVITY'S SAKE)
echo Ww3OUIjU+tk/Mp5pqLTqw69Fa0gl/ip2X+ASD4qrw7SQDFvaM/D6KE03g62EVlwj9B/P5I
echo I8v6Fam9mg6W8AAAARcm9vdEBiNzYwNTU1NTAxMWEBAg==
echo -----END OPENSSH PRIVATE KEY-----
) > ___KAGGLE_PRIVATE_SSH_KEY___
ssh -i ___KAGGLE_PRIVATE_SSH_KEY___ root@0.tcp.us-cal-1.ngrok.io -p 15356 -o ServerAliveInterval=60
```
8) DONE!
