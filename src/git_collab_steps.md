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

git config --global suser.name "kripa"


When cloing using ssh not https. Else there will be issue using  private public key appraoch


 git clone git@github.com:ku064/git_collab.git

 changed from forked git

vim ~/.ssh/config

git@github.com:kripau/git_collab.git

git remote rm origin

git remote add origin git@github-second:kripau/git_collab.git

git remote add origin git@github-COMPANY:Company/testing.git

# this is useful link so added

https://www.freecodecamp.org/news/manage-multiple-github-accounts-the-ssh-way-2dadc30ccaca/


