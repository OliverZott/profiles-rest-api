# Profiles REST API


---
## Tools
- VirtualBox
- Vagrant
- Atom Editor


---
## Start project
- `vagrant up`
- `vagrant ssh`
- `exit`


---
## First Steps
- Initialize Git Repo
  - `git init`
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

## Initialize/Configure/Start Vagrant
- create vagrant file in project folder by:
  `vagrant init ubuntu/bionic64`
- configure as required
  https://www.udemy.com/course/django-python/learn/lecture/6954890#questions/4464262

- in project folder use `vagrant up` which will:
  - download base image (specified in vagrant file)
  - use virtual box to create new virtual machine
  - run provisioning script when it starts machine

- use development server and connect
  - connect to server after vagrant box is started using **SSH** command
  - ssh needed because box is guest operating system (isolated)
  - `vagrant ssh`
  - exit with `exit`
