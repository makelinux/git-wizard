git-wizard - instant git magic and tricks
=====

An interactive git `Command-line interface (CLI)<https://en.wikipedia.org/wiki/Command-line_interface/>` utility for working efficiently.

Git-Wizard's vision: collect git tricks, troubleshooting techniques and git wisdom
under one hat and perform them interactively.

Beginners can enjoy learning git functionality interactively.
Experienced command line git users can save time by using the wizard
to perform frequent operations.

For example, when you have a merge conflict the wizard first suggests
that you run mergetool.

.. contents::
   :local:

Features
****

Fast
----
* Requires minimal key presses to perform the necessary actions.
* Faster then raw git CLI or GUI for many actions.

Comfortable
----
* Displays improved reports.
* Automatically performs routine tasks.

Smart
----
* Prioritizes issues by their importance.
* Filters unsuitable tasks and proposes to perform suitable ones.

For example, the wizard proposes to stage changes only when
there are changed files.

Details
****

Internal checks
----
Each iteration, the wizard checks whether the repository contains collisions,
operations in progress, conflicts, unmerged files,
changes, stashes, ahead/behind commits, and untracked files.

It performs "git fetch" periodically and automatically.

It pronounces some valuable short messages audibly using the espeak application.

Internal actions
----
The wizard uses following commands under the hood: init, status, add,
commit, mergetool, diff, fetch, push, pull, clone, stash, log, clean,
gui and gitk, espeak.

Report
----

Reports the current status of the repository:

git-wizard report::

  root: /home/costa/Dropbox/linux/git-wizard
  conflicted files: 0
  unmerged files: 0
  in progress:
  odified files: 2
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

* Analyze the details of 'in progress' status.
* **You are welcome to request new features and add git tricks**
