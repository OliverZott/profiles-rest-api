# Profiles REST API

## Tools
- VirtualBox
- Vagrant
- Atom Editor

## First Steps
- Initialize Git Repo
- Add README file
- Add .gitignore file
  https://www.toptal.com/developers/gitignore
- Add License file
  https://choosealicense.com/licenses/mit/
- Initial commit
  - `git status`
  - `git add .`
  - `git commit -am "message"`
  - do the following as github suggest:
  - `git remote add ...`
  - `git branch ...`
  - `git push`

- Initialize Remote Git Repo
- Add **SSH public key** for machine to the github repo
  - https://stackoverflow.com/questions/31813080/windows-10-ssh-keys
  - https://www.techrepublic.com/article/how-to-view-your-ssh-keys-in-linux-macos-and-windows/
  - Windows Terminal `ssh-keygen`
  - view `cat ~/ssh/id_rsa.pub` or `type c:\Users\...\.ssh\id_rsa.pub`
  - Add in github with name for machine7

## Initialize Vagrant
- create vagrant file in project folder by:
  `vagrant init ubuntu/bionic64`
