<<<<<<< HEAD
# Data analysis
- Document here the project: STR_project
- Description: Project Description
- Data Source:
- Type of analysis:

Please document the project the better you can.

# Stratup the project

The initial setup.

Create virtualenv and install the project:
```bash
  $ sudo apt-get install virtualenv python-pip python-dev
  $ deactivate; virtualenv ~/venv ; source ~/venv/bin/activate ;\
    pip install pip -U; pip install -r requirements.txt
```

Unittest test:
```bash
  $ make clean install test
```

Check for STR_project in gitlab.com/{group}.
If your project is not set please add it:

- Create a new project on `gitlab.com/{group}/STR_project`
- Then populate it:

```bash
  $ ##   e.g. if group is "{group}" and project_name is "STR_project"
  $ git remote add origin git@gitlab.com:{group}/STR_project.git
  $ git push -u origin master
  $ git push -u origin --tags
```

Functionnal test with a script:
```bash
  $ cd /tmp
  $ STR_project-run
```
# Install
Go to `gitlab.com/{group}/STR_project` to see the project, manage issues,
setup you ssh public key, ...

Create a python3 virtualenv and activate it:
```bash
  $ sudo apt-get install virtualenv python-pip python-dev
  $ deactivate; virtualenv -ppython3 ~/venv ; source ~/venv/bin/activate
```

Clone the project and install it:
```bash
  $ git clone gitlab.com/{group}/STR_project
  $ cd STR_project
  $ pip install -r requirements.txt
  $ make clean install test                # install and test
```
Functionnal test with a script:
```bash
  $ cd /tmp
  $ STR_project-run
```

# Continus integration
## Github
Every push of `master` branch will execute `.github/workflows/pythonpackages.yml` docker jobs.
## Gitlab
Every push of `master` branch will execute `.gitlab-ci.yml` docker jobs.
=======
# STR_project
>>>>>>> d645925b0230670d1090d8b9939b0fc3d98f10e0
