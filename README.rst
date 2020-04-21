git-wizard - interactive talking front end git wrapper script
=====

Wizard's vision: collect git tricks, troubleshooting techniques and git wisdom
under one hat.

git-wizard scans status for your repository and suggests to perform suitable
operations.
Beginners can enjoy interactively learn git functionality.
Experienced command line git users can save they time by using the wizard
to preform recurrent operations.

For example when you have a merge conflict the wizard first of all suggests
to run mergetool.

.. contents::
   :local:

Features
****

Each iteration the wizard checks whether the repository contains collisions,
operations in progress, changes, stashes, ahead/behind commits, untracked files.
Periodically automatically it performs fetch.
Some valuable short messages the wizard tells you audiable via application
espeak.

The wizard uses following commands:

* init
* status
* add
* commit
* mergetool
* diff
* fetch
* push
* pull
* clone
* stash
* log
* clean


Report
----

Just reports current status of the repostory:

git-wizard report

root: /home/costa/Dropbox/linux/git-wizard
unmerged files: 0
in progress:
staged files: 0
modified files: 2
head: master
local branches: 2
remote branches: 3
stashes: 2
commited: 2 minutes ago
remote: origin
fetch age (min): 6
local commits: 3
remote commits: 0
action itemes: 1
gone branches: 0
untracked files: 3

To do
****

* Analize details of 'in progress' status.
* Cleanup 'gone' branches.
* **You are welcome to request new features and add git tricks**
