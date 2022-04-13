# Install

# Configure tooling

`git config --global user.name "[name]"` - Sets the name you want attached to your commit transactions.
`git config --global user.email "[email address]"` - Sets the email you want attached to your commit transactions.
`git config --global color.ui auto` - Enables helpful colorization of command line output.

# Branches

`git branch [branch-name]` - Creates a new branch.
`git checkout [branch-name]` - Switches to the specified branch and updates the working directory.
`git merge [branch]` - Combines the specified branch's history into the current branch. This is usually done in pull requests, but is an important Git operation.
`git branch -d [branch-name]` - Delete the specified branch.

# Create repositories

`git init` - Turn an existing directory into a git repository.
`git clone [url]` - Clone (download) a repository that already exists on GitHub, including all of the files, branches and commits.

# The .gitignore file

Sometimes it may be a good idea to exclude files from being tracked with Git. 
This is typically done in a special file named `.gitignore`.
You can find helpful templates for `.gitignore` files at github.com/github/gitignore

# Synchronize changes

`git fetch` - Downloads all history from the remote tracking branches.
`git merge` - Combines remote tracking branch into current local branch.
`git push` - Uploads all local branch commits to GitHub
`git pull` - Updates your current local working branch with all new commits from the corresponding remote branch on GitHub. `git pull` is a combination of `git fetch` and `git merge`.

---

# Make changes

# Redo commits

# Glossary
