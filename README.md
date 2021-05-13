# Profiles REST API



## DevEnvironment
- VirtualBox
- Vagrant


---
## Start project
- `vagrant up`
- `vagrant ssh`
- `exit`


---
## Structure
 - my_project_folder
   - django_project
   - sub_project_1
   - sub_project_2

- `profiles-rest-api`
  - `preofiles_project`
  - `profiles_api`


# Initial Project Setup
- Initialize Git Repo
  - `git init`
- Add files: 
  - README.md
  - .gitignore  https://www.toptal.com/developers/gitignore
  - LICENSE     https://choosealicense.com/licenses/mit/
- Initial commit
  - `git status`
  - `git add .`
  - `git commit -am "message"`
  - `git remote add ...`  (github suggestion)
  - `git branch ...`
  - `git push`

- Initialize Remote Git Repo
- Add **SSH public key** for machine to the github repo
  - `ssh-keygen` (Windows Terminal)
  - view `cat ~/ssh/id_rsa.pub` or `type c:\Users\...\.ssh\id_rsa.pub`
  - Add in github with name for machine


---
## Initialize/Configure/Start Vagrant
Create vagrant file in project folder (and configure as required):  
  - `vagrant init ubuntu/bionic64`

Dowload base image; run vm; run provisioning script on start  
  - `vagrant up` 

Connect to development server
  - `vagrant ssh`
  - exit with `exit`


---
## Python Virtual Environment
Create virtual environment
- `vagrant@ubuntu-bionic:/vagrant$ python -m venv ~/env`

Activate venv
- `vagrant@ubuntu-bionic:/vagrant$ source ~/env/bin/activate`
- `vagrant@ubuntu-bionic:/vagrant$ deactivate`

---
## Python Packages
- *requiremenets.txt*
- `(env) vagrant@ubuntu-bionic:/vagrant$ pip install -r requirements.txt`