# GIT

`git init`

`git add .`

`git commit -m "first commit"`

`git remote add origin https://github.com/Sarlota-Duskova/freecodecamp.git`

`git pull --rebase origin main`

`git push -f origin main`



#### freecodecamp

`git init`

`git status` - check git status&#x20;

`git checkout -b main` - create and switch to new branch

`git checkout main` - switch to branch main

`touch README.MD`

`git add file_name` - add it to the staging area l

`git commit -m "Initial commit"` - The `-m` stands for "message"

`git log` - Check commit history

`git diff` - see the changes you made with&#x20;

`git branch -d branch_name` - `-d` stands for "delete"

`git rebase main` - You need to update this branch so it has the same commits from `main`, but you can't just merge that branch into this one. You need to `rebase` this branch against `main` to do that

`git merge branch_name` - merge branch

Put your changes aside with `git stash`

View the things you have stashed with `git stash list`

Bring the changes back with `git stash pop`

View the full changes of the latest stash with `git stash show -p`. `-p` stands for "patch".

You can add the latest stash while keeping it in the list with `git stash apply`

You can use the name at the front of each stash (`stash@{#}`)

Use the `git reset` command to travel to any point in your commit history.&#x20;

`git reset HEAD~1`

So when you `reset` to one commit before `HEAD`, it removed the most recent commit, and put all the changes in the working tree. If you used the `--hard` flag with the reset, the changes would have not been added to the working tree and if you used the `--soft` flag, the changes would have been added to the working tree and to staging.

`git revert HEAD` -&#x20;

`git rebase --interactive --root` - `--interactive` rebase that goes back to the `--root` instead of `HEAD~2`,  `--root` means that the rebase will go back to your very first commit.

When you rebase interactively it changes all those hashes, so git sees them as different commits. If you were to try and merge this into `main`, it wouldn't work because they don't share the same history anymore. For this reason, you don't want to do an interactive rebase where you go back passed commits unique to the branch you are on. Fortunately, you can fix this. Enter `git rebase main` to realign the history of the two branches.

`.gitignore` - is a file that ignores files





