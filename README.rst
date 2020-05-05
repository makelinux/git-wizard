git-wizard - instant git magic and tricks
=====

Interactive cli git utility for efficient work

Wizard's vision: collect git tricks, troubleshooting techniques and git wisdom
under one hat and perform them interactively in dialogue.

Beginners can enjoy interactively learn git functionality.
Experienced command line git users can save they time by using the wizard
to preform frequent operations.

For example when you have a merge conflict the wizard first of all suggests
you to run mergetool.

.. contents::
   :local:

Features
****

Fast
----
* Requires minimal key presses to perform requires actions.
* Faster then raw git cli or gui for many actions

Comfortable
----
* Prints improved reports
* Takes on routine tasks automatically

Smart
----
* Prioritizes issues accordingly importance
* Filters unstable and proposes to perform suitable tasks

For example the wizard proposes add changes to stage only when
there are changed files.

Details
****

Internal checks
----
Each iteration the wizard checks whether the repository contains collisions,
operations in progress, conflicts, unmerged files,
changes, stashes, ahead/behind commits, untracked files.
Periodically automatically it performs fetch.
Some valuable short messages the wizard tells you audible via application
espeak.

Internal actions
----
The wizard uses following commands under the hood: init, status, add,
commit, mergetool, diff, fetch, push, pull, clone, stash, log, clean,
gui and gitk, espeak

Report
----

Just reports current status of the repository:

git-wizard report::

  root: /home/costa/Dropbox/linux/git-wizard
  conflicted files: 0
  unmerged files: 0
  in progress:
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

Other features
----
* Cleans up 'gone' branches and helps to keep your workspace tidy.

To do
****

* Analize details of 'in progress' status.
* **You are welcome to request new features and add git tricks**
