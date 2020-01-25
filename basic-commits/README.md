# Git Kata: Basic Commits
This kata will introduce you to the `git add` and `git commit` commands.

This is a very introductory kata. if you have used `git status`, `git log --oneline --graph`, `git add` and `git commit` extensively you should probably skip it.

You can look at the bottom of this file, if you have not yet done basic git configuration.

## Setup:

1. Run `. setup.sh` (or `.\setup.ps1` in PowerShell)

## The task

1. Use `git status` to see which branch you are on.
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean

2. What does `git log` look like?
commit f8712d5c4df74fa0d49c8cc9ba3b1a5b2c571072 (HEAD -> master, origin/master, origin/HEAD)
Author: Frank Theile <ftheile@grundfos.com>
Date:   Mon Dec 9 10:30:13 2019 +0100

    Add missing shebang in squashing/setup.sh
    
    `setup.sh` should be executable according to the instructions given in README.md

commit e060df632bf4799da9aa1c0092640563acf84588
Author: Adam Matan <adamatan@users.noreply.github.com>
Date:   Wed Dec 4 07:46:31 2019 +0200

    Word ordering

commit 6ccb85882dc12fb0b26acd65bead2fc7da57a187
Author: Frank Theile <ftheile@grundfos.com>
Date:   Wed Nov 27 08:24:29 2019 +0100

    Mention `less` in SHELL-BASICS.md
    
    Helpful alternative to `cat` for long files.

3. Create a file
vim tempFile.txt

4. What does the output from `git status` look like now?
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	tempFile.txt

nothing added to commit but untracked files present (use "git add" to track)

5. `add` the file to the staging area
git add tempFile.txt

6. How does `git status` look now?
        On branch master

        No commits yet

        Changes to be committed:
          (use "git rm --cached <file>..." to unstage)
                        new file:   tempFile.txt

7. `commit` the file to the repository
[master b937af2] Committing the text file.
 1 file changed, 2 insertions(+)
 create mode 100644 basic-commits/tempFile.txt

8. How does `git status` look now?
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

9. Change the content of the file you created earlier
vim tempFile.txt

10. What does `git status` look like now?
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   tempFile.txt

no changes added to commit (use "git add" and/or "git commit -a")

11. `add` the file change
git add tempFile.txt

12. What does `git status` look like now?
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	modified:   tempFile.txt

13. Change the file again
 vim tempFile.txt

14. Make a `commit`
[master c1a2481] Made a change!
 1 file changed, 2 insertions(+)

15. What does the `status` look like now? The `log`?
status:
On branch master
Your branch is ahead of 'origin/master' by 2 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean


log:
commit c1a24814c0a7a97d1f8c50a5b94e195565fd17ac (HEAD -> master)
Author: mahasheikh89 <34201572+mahasheikh89@users.noreply.github.com>
Date:   Fri Jan 24 21:58:43 2020 -0800

    Made a change!

commit b937af22718501bbf0cfb2201dae775cfe2adfb1
Author: mahasheikh89 <34201572+mahasheikh89@users.noreply.github.com>
Date:   Fri Jan 24 21:56:41 2020 -0800

    Committing the text file.

commit f8712d5c4df74fa0d49c8cc9ba3b1a5b2c571072 (origin/master, origin/HEAD)
Author: Frank Theile <ftheile@grundfos.com>
Date:   Mon Dec 9 10:30:13 2019 +0100

    Add missing shebang in squashing/setup.sh
    
    `setup.sh` should be executable according to the instructions given in README.md

commit e060df632bf4799da9aa1c0092640563acf84588
Author: Adam Matan <adamatan@users.noreply.github.com>

16. Commit the newest change

## Useful commands
- `git add`
- `git commit`
- `git commit -m "My commit message"`
- `git log`
- `git log -n 5`
- `git log --oneline`
- `git log --oneline --graph`
- `touch filename` to create a file (or `sc filename ''` in PowerShell)
- `echo content > file` to overwrite file with content (or `sc filename 'content'` in PowerShell)
- `echo content >> file` to append file with content (or `ac filename 'content'` in PowerShell)


## Git Initial Configuration
1. `git config --global user.name "John Doe"`
1. `git config --global user.email "johndoe@example.com`

For the vim scared:
- `git config --global core.editor nano`

For the windows peeps:
- `git config --global core.editor notepad`

Other editor options:
- `git config --global core.editor "atom --wait"`
- `git config --global core.editor "'C:/Program Files/Notepad++/notepad++.exe' -multiInst"`
