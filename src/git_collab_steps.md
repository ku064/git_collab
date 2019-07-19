### clone the file to local repo

git clone https://github.com/ku064/git_collab.git

Create a text file and save as get_collab_steps.md

git add .  # to add the file from working area to staging area


generate ssh key in private machine

ssh-keygen -t rsa -b 4096 -C kripaupreti064@gmail.com

bpcopy < ~/.ssh/ku064_rsa.pub

# set the host

Host github.com
  HostName github.com
  User git
  IdentityFile ~/.ssh/ku064_rsa

git config --global user.email "kripaupreti064@gmail.com"
git config --global user.name "kripa"


When cloing using ssh not https. Else there will be issue using  private public key appraoch


 git clone git@github.com:ku064/git_collab.git

 changed from forked git

vim ~/.ssh/config

git@github.com:kripau/git_collab.git

git remote add origin git@github-second:kripau/git_collab.git
