<!-- TOC -->

- [Contributing](#contributing)
- [About VSCode](#about-vscode)

<!-- TOC -->

# Contributing

> Configure authentication on your account to use the SSH protocol instead of HTTP. See this [tutorial](https://confluence.atlassian.com/bitbucketserver/ssh-access-keys-for-system-use-776639781.html)

* Install the [requirements](REQUIREMENTS.md).

* Create a fork this repository.

* Clone the forked repository to your local system:

```bash
git clone URL_FORKED_REPOSITORY
```

* Add the address for the remote original repository:

```bash
git remote -v
git remote add upstream git@github.com:rbulbow/docker-class
git remote -v
```

* Create a branch. Example:

```bash
git checkout -b BRANCH_NAME
```

* Make sure you are on the correct branch using the following command. The branch in use contains the '*' before the name.

```bash
git branch
```

* Make your changes and tests to the new branch. See the section [Updating this image](README.md#updating-this-image).
* Commit the changes to the branch.
* Push files to repository remote with command:

```bash
git push --set-upstream origin BRANCH_NAME
```

* Create a Pull Request (PR) for the `main` branch of the repository. Watch this [tutorial](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request-from-a-fork).
* Update the content with the suggestions of the reviewer (if necessary).
* After your pull request has been approved and merged, update your local clone:

```bash
git checkout main
git pull upstream main
```

* Clean up after your pull request is merged with command:

```bash
git branch -d BRANCH_NAME
```

* Then you can update the `main` branch in your forked repository.

```bash
git push origin main
```

* And push the deletion of the feature branch to your GitHub repository with command:

```bash
git push --delete origin BRANCH_NAME
```

* To keep your fork in sync with the original repository, use these commands:

```bash
git pull upstream main
git push origin main
```

Reference:

* https://blog.scottlowe.org/2015/01/27/using-fork-branch-git-workflow/

