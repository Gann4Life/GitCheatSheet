# Git Cheat Sheet

Git is the open source distributed version control system that facilitates GitHub activities on your laptop or desktop. This cheat sheet summarizes commonly used Git command line instructions for quick reference.

---

<h3 name="index">Index</h3>

[![Button](https://shields.io/badge/Go%20to-Install-black?style=flat)](#install)

[![Button](https://shields.io/badge/Go%20to-Create%20repositories-black?style=flat)](#create-repositories)

[![Button](https://shields.io/badge/Go%20to-Configure%20tooling-black?style=flat)](#configure-tooling)

[![Button](https://shields.io/badge/Go%20to-The%20.gitignore%20file-black?style=flat)](#gitignore)

[![Button](https://shields.io/badge/Go%20to-Branches-black?style=flat)](#branches)

[![Button](https://shields.io/badge/Go%20to-Synchronize%20changes-black?style=flat)](#synchronize-changes)

[![Button](https://shields.io/badge/Go%20to-Make%20changes-black?style=flat)](#make-changes)

[![Button](https://shields.io/badge/Go%20to-Redo%20changes-black?style=flat)](#redo-changes)

---

<h3 name="install">Install</h3>

* [**GitHub for Windows**](https://windows.github.com)<br>
* [**GitHub for Mac**](https://mac.github.com)<br>
* [**Git for All Platforms**](https://git-scm.com)

[![Button](https://shields.io/badge/Go%20to-Index-black?style=flat)](#index)

<h3 name="create-repositories">Create repositories</h3>

When starting out with a new repository, you only need to do it once; either locally, then push to GitHub, or by cloning an existing repository.

> `$ git init`<br>
> Turn an existing directory into a git repository.

> `$ git clone [url]`<br>
> Clone (download) a repository that already exists on GitHub, including all of the files, branches and commits.

[![Button](https://shields.io/badge/Go%20to-Index-black?style=flat)](#index)

<h3 name="configure-tooling">Configure tooling</h3>

Configure user information for all local repositories.

> `$ git config --global user.name "[name]"`<br>
> Sets the name you want attached to your commit transactions.

> `git config --global user.email "[email address]"`<br>
> Sets the email you want attached to your commit transactions.

> `$ git config --global color.ui auto`<br>
> Enables helpful colorization of command line output.

[![Button](https://shields.io/badge/Go%20to-Index-black?style=flat)](#index)

<h3 name="gitignore">The .gitignore file</h3>

Sometimes it may be a good idea to exclude files from being tracked with Git. This is typically done in a special file named `.gitignore`. You can find helpful templates for `.gitignore` files at https://github.com/github/gitignore.

[![Button](https://shields.io/badge/Go%20to-Index-black?style=flat)](#index)

<h3 name="branches">Branches</h3>

Branches are an important part of working with Git. Any commits you make will be made on the branch you're currently "checked out" to. Use `git status` to see which branch that is.

> `$ git branch [branch-name]`<br>
> Creates a new branch.

> `$ git checkout [branch-name]`<br>
> Switches to the specified branch and updates the working directory.

> `$ git merge [branch]`<br>
> Combines the specified branch's history into the current branch. This is usually done in pull requests, but is an important Git operation.

> `$ git branch -d [branch-name]`<br>
> Delete the specified branch.

[![Button](https://shields.io/badge/Go%20to-Index-black?style=flat)](#index)

<h3 name="synchronize-changes">Synchronize changes</h3>

> `$ git fetch`<br>
> Downloads all history from the remote tracking branches.

> `$ git merge`<br>
> Combines remote tracking branch into current local branch.

> `$ git push`<br>
>Uploads all local branch commits to GitHub.

> `$ git pull`<br>
> Updates your current local working branch with all new commits from the corresponding remote branch on GitHub. `git pull` is a combination of `git fetch` and `git merge`.

[![Button](https://shields.io/badge/Go%20to-Index-black?style=flat)](#index)

---

<h3 name="make-changes">Make changes</h3>

Browse and inspect the evolution of project files.

> `$ git log`<br>
> Lists version history for the current branch.

> `$ git log --follow [file]`<br>
> Lists version history for a file, including renames.

> `$ git diff [first-branch]...[second-branch]`<br>
> Shows content differences between two branches.

> `$ git show [commit]`<br>
> Outputs metadata and content changes of the specified commit.

> `$ git add [file]`<br>
> Snapshots the file in preparation for versioning.

> `$ git commit -m "[descriptive message]"`<br>
> Records file snapshots permanently in version history.

[![Button](https://shields.io/badge/Go%20to-Index-black?style=flat)](#index)

<h3 name="redo-commits">Redo commits</h3>

Erase mistakes and craft replacement history.

> `$ git reset [commit]`<br>
> Undoes all commits after [commit], preserving changes locally.

> `$ git reset --hard [commit]`<br>
> Discards all history and changes back to the specified commit.

CAUTION! Changing history can have nasty side effects. If you need to change commits that exist on GitHub (the remote), proceed with caution. If you need help, reach out at github.community or contact support.

[![Button](https://shields.io/badge/Go%20to-Index-black?style=flat)](#index)

---

<h3 name="glossary">Glossary</h3>

**git**: an open source, distributed version-control system.

**GitHub**: a platform for hosting and collaborating on Git repositories.

**commit**: a Git object, a snapshot of your entire repository compressed into a SHA.

**branch**: a lightweight movable pointer to a commit.

**clone**: a local version of a repository, including all commits and branches.

**remote**: a common repository on GitHub that all team member use to exchange their changes.

**fork**: a copy of a repository on GitHub owned by a different user.

**pull request**: a place to compare and discuss the differences introduced on a branch with reviews, comments, integrated tests, and more.

**HEAD**: representing your current working directory, the HEAD pointer can be moved to different branches, tags or commits when using `git checkout`.

[![Button](https://shields.io/badge/Go%20to-Index-black?style=flat)](#index)