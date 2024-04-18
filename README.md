# General

**Dev environment-related useful notes:**

* **Create an environment to a specific python version:** `virtualenv causalityEnv3.10 -p python3.10`
* **Activate the created environment:** `.\causalityEnv3.10\Scripts\activate`
* **Get the package list:** `python -m pip freeze > requirements3.10.txt`
* **Install the package list:** `python -m pip install -r requirements3.10.txt`
* **Deactivate the environment:** `deactivate`

**git related useful commands:**

* Create tag: `git tag `<tagname>
* Push tags: `git push origin --tags`
* Move tags, steps:
  * git tag -d <tagname>                  # delete the old tag locally
  * git push origin :refs/tags/<tagname>  # delete the old tag remotely
  * git tag <tagname> <commitId>          # make a new tag locally
  * git push origin <tagname>             # push the new local tag to the remote
