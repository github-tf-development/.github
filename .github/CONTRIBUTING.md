# Contributing

## 1. Install Git CLI
please follow https://git-scm.com/downloads to install git cli on your preferred machine. create git pat token with commits rights and save it somewhere safe place. you can use git credentails manager to save it.

## 2. Request for changes/ Pull Requests
You first need to create a fork of the [repo-name](https://github.com/org-name/repo-name) repository to commit your changes to it. Methods to fork a repository can be found in the [GitHub Documentation](https://docs.github.com/en/get-started/quickstart/fork-a-repo).

## 3. Clone the repo
Then add your fork as a local project:

```sh
# Using HTTPS
git clone https://YOUR-USERNAME@github.com/org-name/repo-name.git


# Using SSH
git clone git@github.com:org-name/repo-name.git
```
This will prompt to enter password/token
> [Which remote URL should be used ?](https://docs.github.com/en/get-started/getting-started-with-git/about-remote-repositories)

Then, go to your local folder

```sh
cd repo-name
```

Add git remote controls :

```sh
# Using HTTPS
git remote add fork https://github.com/YOUR-USERNAME/repo-name.git
git remote add upstream https://github.com/org-name/repo-name.git


# Using SSH
git remote add fork git@github.com:YOUR-USERNAME/repo-name.git
git remote add upstream git@github.com/org-name/repo-name.git
```

You can now verify that you have your two git remotes:

```sh
git remote -v
```

## Receive remote updates
In view of staying up to date with the central repository :

```sh
git pull upstream master
```

## Choose a base branch
Before starting development, you need to know which branch to base your modifications/additions on. When in doubt, use main/prod.

| Type of change                |           | Branches              |
| :------------------           |:---------:| ---------------------:|
| Documentation                 |           | `dev`              |
| Bug fixes                     |           | `dev`  || `main`   |
| New features                  |           | `dev`              |
| New issues models             |           | `YOUR-USERNAME:patch` |

```sh
# Switch to the desired branch
git switch dev

# Pull down any upstream changes
git pull

# Create a new branch to work on
git switch --create patch/1234-name-issue
```
Any type to secret/access keys must not be pushed to any repo user GitHub secrets or other tools to store them

Commit your changes, then push the branch to your fork with `git push -u fork` and open a pull request on [repo-name](https://github.com/org-name/repo-name.git) following the template provided. Once all the changes are validated raise a pull request to merge your patch branch into dev and then to main/prod.
