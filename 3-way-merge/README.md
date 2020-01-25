# Git Kata: 3-Way Merge

## Setup

1. Run `. setup.sh` (or `.\setup.ps1` in PowerShell)

## The task
You again live in your own branch, this time we will be doing a bit of juggling with branches, to show how lightweight branches are in git.

1. Create a branch called greeting and check it out
2. Edit the greeting.txt to contain your favorite greeting
3. Add greeting.txt files to the staging area
4. Commit
5. Switch back to the master branch
6. Create a file README.md with information about this repository
7. Add the README.md file to staging area and make the commit
8. What is the output of `git log --oneline --graph --all`?
On branch master
Your branch is ahead of 'origin/master' by 3 commits.
  (use "git push" to publish your local commits)

Changes not staged for commit:
	modified:   ../basic-commits/README.md

Untracked files:
	../.DS_Store
	../basic-commits/.DS_Store

no changes added to commit
Mahas-MacBook-Pro:3-way-merge mahasheikh$ git log --oneline -- graph --all
Mahas-MacBook-Pro:3-way-merge mahasheikh$ git log --oneline --graph --all
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
* f56e566 Added useful commands section to amend/README.
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
* f56e566 Added useful commands section to amend/README.
* 3b9e5ea Added to Merge Mergesort README
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
* f56e566 Added useful commands section to amend/README.
* 3b9e5ea Added to Merge Mergesort README
* 0f430e6 Use makerepo function
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
* f56e566 Added useful commands section to amend/README.
* 3b9e5ea Added to Merge Mergesort README
* 0f430e6 Use makerepo function
* 9e8ed9d Set theme jekyll-theme-midnight
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
* f56e566 Added useful commands section to amend/README.
* 3b9e5ea Added to Merge Mergesort README
* 0f430e6 Use makerepo function
* 9e8ed9d Set theme jekyll-theme-midnight
*   00a9e17 Merge pull request #201 from Natasha2001/master
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
* f56e566 Added useful commands section to amend/README.
* 3b9e5ea Added to Merge Mergesort README
* 0f430e6 Use makerepo function
* 9e8ed9d Set theme jekyll-theme-midnight
*   00a9e17 Merge pull request #201 from Natasha2001/master
|\  
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
* f56e566 Added useful commands section to amend/README.
* 3b9e5ea Added to Merge Mergesort README
* 0f430e6 Use makerepo function
* 9e8ed9d Set theme jekyll-theme-midnight
*   00a9e17 Merge pull request #201 from Natasha2001/master
|\  
| * 59d5e43 Introduction to github
* |   03a672f Merge pull request #202 from atombrella/rebase_source
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
* f56e566 Added useful commands section to amend/README.
* 3b9e5ea Added to Merge Mergesort README
* 0f430e6 Use makerepo function
* 9e8ed9d Set theme jekyll-theme-midnight
*   00a9e17 Merge pull request #201 from Natasha2001/master
|\  
| * 59d5e43 Introduction to github
* |   03a672f Merge pull request #202 from atombrella/rebase_source
|\ \  
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
* f56e566 Added useful commands section to amend/README.
* 3b9e5ea Added to Merge Mergesort README
* 0f430e6 Use makerepo function
* 9e8ed9d Set theme jekyll-theme-midnight
*   00a9e17 Merge pull request #201 from Natasha2001/master
|\  
| * 59d5e43 Introduction to github
* |   03a672f Merge pull request #202 from atombrella/rebase_source
|\ \  
| * | 46c519b Added exec-flag to setup.sh script, and fixed syntax error with sh:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
* f56e566 Added useful commands section to amend/README.
* 3b9e5ea Added to Merge Mergesort README
* 0f430e6 Use makerepo function
* 9e8ed9d Set theme jekyll-theme-midnight
*   00a9e17 Merge pull request #201 from Natasha2001/master
|\  
| * 59d5e43 Introduction to github
* |   03a672f Merge pull request #202 from atombrella/rebase_source
|\ \  
| * | 46c519b Added exec-flag to setup.sh script, and fixed syntax error with shebang.
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
* f56e566 Added useful commands section to amend/README.
* 3b9e5ea Added to Merge Mergesort README
* 0f430e6 Use makerepo function
* 9e8ed9d Set theme jekyll-theme-midnight
*   00a9e17 Merge pull request #201 from Natasha2001/master
|\  
| * 59d5e43 Introduction to github
* |   03a672f Merge pull request #202 from atombrella/rebase_source
|\ \  
| * | 46c519b Added exec-flag to setup.sh script, and fixed syntax error with shebang.
| |/  
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
* f56e566 Added useful commands section to amend/README.
* 3b9e5ea Added to Merge Mergesort README
* 0f430e6 Use makerepo function
* 9e8ed9d Set theme jekyll-theme-midnight
*   00a9e17 Merge pull request #201 from Natasha2001/master
|\  
| * 59d5e43 Introduction to github
* |   03a672f Merge pull request #202 from atombrella/rebase_source
|\ \  
| * | 46c519b Added exec-flag to setup.sh script, and fixed syntax error with shebang.
| |/  
* |   e231eef Merge pull request #200 from atombrella/git_ignore_track_ignored
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
* f56e566 Added useful commands section to amend/README.
* 3b9e5ea Added to Merge Mergesort README
* 0f430e6 Use makerepo function
* 9e8ed9d Set theme jekyll-theme-midnight
*   00a9e17 Merge pull request #201 from Natasha2001/master
|\  
| * 59d5e43 Introduction to github
* |   03a672f Merge pull request #202 from atombrella/rebase_source
|\ \  
| * | 46c519b Added exec-flag to setup.sh script, and fixed syntax error with shebang.
| |/  
* |   e231eef Merge pull request #200 from atombrella/git_ignore_track_ignored
|\ \  
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
* f56e566 Added useful commands section to amend/README.
* 3b9e5ea Added to Merge Mergesort README
* 0f430e6 Use makerepo function
* 9e8ed9d Set theme jekyll-theme-midnight
*   00a9e17 Merge pull request #201 from Natasha2001/master
|\  
| * 59d5e43 Introduction to github
* |   03a672f Merge pull request #202 from atombrella/rebase_source
|\ \  
| * | 46c519b Added exec-flag to setup.sh script, and fixed syntax error with shebang.
| |/  
* |   e231eef Merge pull request #200 from atombrella/git_ignore_track_ignored
|\ \  
| * | 301f919 Added exercise about excluding something from .gitignore
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
* f56e566 Added useful commands section to amend/README.
* 3b9e5ea Added to Merge Mergesort README
* 0f430e6 Use makerepo function
* 9e8ed9d Set theme jekyll-theme-midnight
*   00a9e17 Merge pull request #201 from Natasha2001/master
|\  
| * 59d5e43 Introduction to github
* |   03a672f Merge pull request #202 from atombrella/rebase_source
|\ \  
| * | 46c519b Added exec-flag to setup.sh script, and fixed syntax error with shebang.
| |/  
* |   e231eef Merge pull request #200 from atombrella/git_ignore_track_ignored
|\ \  
| * | 301f919 Added exercise about excluding something from .gitignore
| |/  
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
* f56e566 Added useful commands section to amend/README.
* 3b9e5ea Added to Merge Mergesort README
* 0f430e6 Use makerepo function
* 9e8ed9d Set theme jekyll-theme-midnight
*   00a9e17 Merge pull request #201 from Natasha2001/master
|\  
| * 59d5e43 Introduction to github
* |   03a672f Merge pull request #202 from atombrella/rebase_source
|\ \  
| * | 46c519b Added exec-flag to setup.sh script, and fixed syntax error with shebang.
| |/  
* |   e231eef Merge pull request #200 from atombrella/git_ignore_track_ignored
|\ \  
| * | 301f919 Added exercise about excluding something from .gitignore
| |/  
* |   dfcb536 Merge pull request #196 from brent-clark-SED-Sw-Mgr/add-to-basic-c:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
* f56e566 Added useful commands section to amend/README.
* 3b9e5ea Added to Merge Mergesort README
* 0f430e6 Use makerepo function
* 9e8ed9d Set theme jekyll-theme-midnight
*   00a9e17 Merge pull request #201 from Natasha2001/master
|\  
| * 59d5e43 Introduction to github
* |   03a672f Merge pull request #202 from atombrella/rebase_source
|\ \  
| * | 46c519b Added exec-flag to setup.sh script, and fixed syntax error with shebang.
| |/  
* |   e231eef Merge pull request #200 from atombrella/git_ignore_track_ignored
|\ \  
| * | 301f919 Added exercise about excluding something from .gitignore
| |/  
* |   dfcb536 Merge pull request #196 from brent-clark-SED-Sw-Mgr/add-to-basic-commits-readme
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
* f56e566 Added useful commands section to amend/README.
* 3b9e5ea Added to Merge Mergesort README
* 0f430e6 Use makerepo function
* 9e8ed9d Set theme jekyll-theme-midnight
*   00a9e17 Merge pull request #201 from Natasha2001/master
|\  
| * 59d5e43 Introduction to github
* |   03a672f Merge pull request #202 from atombrella/rebase_source
|\ \  
| * | 46c519b Added exec-flag to setup.sh script, and fixed syntax error with shebang.
| |/  
* |   e231eef Merge pull request #200 from atombrella/git_ignore_track_ignored
|\ \  
| * | 301f919 Added exercise about excluding something from .gitignore
| |/  
* |   dfcb536 Merge pull request #196 from brent-clark-SED-Sw-Mgr/add-to-basic-commits-readme
|\ \  
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
* f56e566 Added useful commands section to amend/README.
* 3b9e5ea Added to Merge Mergesort README
* 0f430e6 Use makerepo function
* 9e8ed9d Set theme jekyll-theme-midnight
*   00a9e17 Merge pull request #201 from Natasha2001/master
|\  
| * 59d5e43 Introduction to github
* |   03a672f Merge pull request #202 from atombrella/rebase_source
|\ \  
| * | 46c519b Added exec-flag to setup.sh script, and fixed syntax error with shebang.
| |/  
* |   e231eef Merge pull request #200 from atombrella/git_ignore_track_ignored
|\ \  
| * | 301f919 Added exercise about excluding something from .gitignore
| |/  
* |   dfcb536 Merge pull request #196 from brent-clark-SED-Sw-Mgr/add-to-basic-commits-readme
|\ \  
| * | 168599d Added more explanatory text to basic-commits/README
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
* f56e566 Added useful commands section to amend/README.
* 3b9e5ea Added to Merge Mergesort README
* 0f430e6 Use makerepo function
* 9e8ed9d Set theme jekyll-theme-midnight
*   00a9e17 Merge pull request #201 from Natasha2001/master
|\  
| * 59d5e43 Introduction to github
* |   03a672f Merge pull request #202 from atombrella/rebase_source
|\ \  
| * | 46c519b Added exec-flag to setup.sh script, and fixed syntax error with shebang.
| |/  
* |   e231eef Merge pull request #200 from atombrella/git_ignore_track_ignored
|\ \  
| * | 301f919 Added exercise about excluding something from .gitignore
| |/  
* |   dfcb536 Merge pull request #196 from brent-clark-SED-Sw-Mgr/add-to-basic-commits-readme
|\ \  
| * | 168599d Added more explanatory text to basic-commits/README
| |/  
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
* f56e566 Added useful commands section to amend/README.
* 3b9e5ea Added to Merge Mergesort README
* 0f430e6 Use makerepo function
* 9e8ed9d Set theme jekyll-theme-midnight
*   00a9e17 Merge pull request #201 from Natasha2001/master
|\  
| * 59d5e43 Introduction to github
* |   03a672f Merge pull request #202 from atombrella/rebase_source
|\ \  
| * | 46c519b Added exec-flag to setup.sh script, and fixed syntax error with shebang.
| |/  
* |   e231eef Merge pull request #200 from atombrella/git_ignore_track_ignored
|\ \  
| * | 301f919 Added exercise about excluding something from .gitignore
| |/  
* |   dfcb536 Merge pull request #196 from brent-clark-SED-Sw-Mgr/add-to-basic-commits-readme
|\ \  
| * | 168599d Added more explanatory text to basic-commits/README
| |/  
* |   a5dbbc6 Merge pull request #193 from atombrella/git_attributes
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
* f56e566 Added useful commands section to amend/README.
* 3b9e5ea Added to Merge Mergesort README
* 0f430e6 Use makerepo function
* 9e8ed9d Set theme jekyll-theme-midnight
*   00a9e17 Merge pull request #201 from Natasha2001/master
|\  
| * 59d5e43 Introduction to github
* |   03a672f Merge pull request #202 from atombrella/rebase_source
|\ \  
| * | 46c519b Added exec-flag to setup.sh script, and fixed syntax error with shebang.
| |/  
* |   e231eef Merge pull request #200 from atombrella/git_ignore_track_ignored
|\ \  
| * | 301f919 Added exercise about excluding something from .gitignore
| |/  
* |   dfcb536 Merge pull request #196 from brent-clark-SED-Sw-Mgr/add-to-basic-commits-readme
|\ \  
| * | 168599d Added more explanatory text to basic-commits/README
| |/  
* |   a5dbbc6 Merge pull request #193 from atombrella/git_attributes
|\ \  
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
* f56e566 Added useful commands section to amend/README.
* 3b9e5ea Added to Merge Mergesort README
* 0f430e6 Use makerepo function
* 9e8ed9d Set theme jekyll-theme-midnight
*   00a9e17 Merge pull request #201 from Natasha2001/master
|\  
| * 59d5e43 Introduction to github
* |   03a672f Merge pull request #202 from atombrella/rebase_source
|\ \  
| * | 46c519b Added exec-flag to setup.sh script, and fixed syntax error with shebang.
| |/  
* |   e231eef Merge pull request #200 from atombrella/git_ignore_track_ignored
|\ \  
| * | 301f919 Added exercise about excluding something from .gitignore
| |/  
* |   dfcb536 Merge pull request #196 from brent-clark-SED-Sw-Mgr/add-to-basic-commits-readme
|\ \  
| * | 168599d Added more explanatory text to basic-commits/README
| |/  
* |   a5dbbc6 Merge pull request #193 from atombrella/git_attributes
|\ \  
| * \   10665da Merge branch 'master' into git_attributes
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
* f56e566 Added useful commands section to amend/README.
* 3b9e5ea Added to Merge Mergesort README
* 0f430e6 Use makerepo function
* 9e8ed9d Set theme jekyll-theme-midnight
*   00a9e17 Merge pull request #201 from Natasha2001/master
|\  
| * 59d5e43 Introduction to github
* |   03a672f Merge pull request #202 from atombrella/rebase_source
|\ \  
| * | 46c519b Added exec-flag to setup.sh script, and fixed syntax error with shebang.
| |/  
* |   e231eef Merge pull request #200 from atombrella/git_ignore_track_ignored
|\ \  
| * | 301f919 Added exercise about excluding something from .gitignore
| |/  
* |   dfcb536 Merge pull request #196 from brent-clark-SED-Sw-Mgr/add-to-basic-commits-readme
|\ \  
| * | 168599d Added more explanatory text to basic-commits/README
| |/  
* |   a5dbbc6 Merge pull request #193 from atombrella/git_attributes
|\ \  
| * \   10665da Merge branch 'master' into git_attributes
| |\ \  
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
* f56e566 Added useful commands section to amend/README.
* 3b9e5ea Added to Merge Mergesort README
* 0f430e6 Use makerepo function
* 9e8ed9d Set theme jekyll-theme-midnight
*   00a9e17 Merge pull request #201 from Natasha2001/master
|\  
| * 59d5e43 Introduction to github
* |   03a672f Merge pull request #202 from atombrella/rebase_source
|\ \  
| * | 46c519b Added exec-flag to setup.sh script, and fixed syntax error with shebang.
| |/  
* |   e231eef Merge pull request #200 from atombrella/git_ignore_track_ignored
|\ \  
| * | 301f919 Added exercise about excluding something from .gitignore
| |/  
* |   dfcb536 Merge pull request #196 from brent-clark-SED-Sw-Mgr/add-to-basic-commits-readme
|\ \  
| * | 168599d Added more explanatory text to basic-commits/README
| |/  
* |   a5dbbc6 Merge pull request #193 from atombrella/git_attributes
|\ \  
| * \   10665da Merge branch 'master' into git_attributes
| |\ \  
| |/ /  
:...skipping...
* 7fd4a0c (HEAD -> master) I committed.
* c1a2481 (greeting) Made a change!
* b937af2 Committing the text file.
* f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md
* c9df4ca Added to The task in reverted-merge/README.md
* e52649c Added to The task in merge-conflict/README.md
* ac8f6c2 Added The task to commit-on-wrong-branch/README.md
* 2e29b3b Added the task section to bad-commit/README.md
* 66f5b27 Added useful commands and more to reset/README
* 8100f96 Add clone step to README Gif
* ee01d2c Added to the task in reorder-the-history/README.
* f56e566 Added useful commands section to amend/README.
* 3b9e5ea Added to Merge Mergesort README
* 0f430e6 Use makerepo function
* 9e8ed9d Set theme jekyll-theme-midnight
*   00a9e17 Merge pull request #201 from Natasha2001/master
|\  
| * 59d5e43 Introduction to github
* |   03a672f Merge pull request #202 from atombrella/rebase_source
|\ \  
| * | 46c519b Added exec-flag to setup.sh script, and fixed syntax error with shebang.
| |/  
* |   e231eef Merge pull request #200 from atombrella/git_ignore_track_ignored
|\ \  
| * | 301f919 Added exercise about excluding something from .gitignore
| |/  
* |   dfcb536 Merge pull request #196 from brent-clark-SED-Sw-Mgr/add-to-basic-commits-readme
|\ \  
| * | 168599d Added more explanatory text to basic-commits/README
| |/  
* |   a5dbbc6 Merge pull request #193 from atombrella/git_attributes
|\ \  
| * \   10665da Merge branch 'master' into git_attributes
| |\ \  
| |/ /  
|/| | 

9. Diff the branches
diff --git a/3-way-merge/exercise/greeting.txt b/3-way-merge/exercise/greeting.txt
new file mode 100644
index 0000000..f48f659
--- /dev/null
+++ b/3-way-merge/exercise/greeting.txt
@@ -0,0 +1 @@
+hello seyonara

10. Merge the greeting branch into master
Already up to date.

## Useful commands
- `git branch`
- `git branch <branch-name>`
- `git branch -d <branch-name>`
- `git checkout <branch-name>`
- `git checkout -b <branch-name>`
- `git branch -v`
- `git add`
- `git commit`
- `git commit -m`
- `git merge <branchA> <branchB>`
- `git diff <branchA> <branchB>`
- `git log --oneline --graph --all`
