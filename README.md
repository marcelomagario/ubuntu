# ubuntu
Important tutorials


## Step 1: Generating a new SSH key

ssh-keygen -t rsa -b 4096 -C "email@gmail.com"


## Step 2: Adding your SSH key to ssh-agent

eval "$(ssh-agent -s)"

ssh-add ~/.ssh/id_rsa


## Step 4: Add your key to GitHub

In order to get our key, use the following command

cat ~/.ssh/id_rsa.pub

Then copy the content (starting from ssh-rsa). 

## ON GITHUB:
SETTINGS -> select SSH and GPG keys --> NEW SSH KEY

Under the title section, add a name to your key. Then in the key section, paste the key that we copied from our terminal. Finally, click on Add SSH key
