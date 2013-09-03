Convention
==========

> A convention is a set of agreed, stipulated, or generally accepted standards,
> norms, social norms, or criteria, often taking the form of a custom.
> ~ [Wikipedia][1]


Write a feature
---------------

Create a local feature branch based off master.

    git checkout master
    git pull
    git checkout -b <BRANCH-NAME>

Prefix the branch name with your initials.

Rebase frequently to incorporate upstream changes.

    git fetch origin
    git rebase origin/master

Resolve conflicts. When feature is complete and tests pass, stage the changes.

    git add --all

When you've staged the changes, commit them.

    git status
    git commit --verbose

Write a [good commit message][2]. Example format:

    Present-tense summary under 50 characters

    * More information about commit (under 72 characters).
    * More information about commit (under 72 characters).

    http://project.management-system.com/ticket/123

Share your branch.

    git push origin <BRANCH-NAME>

Submit a [GitHub pull request][3].

Ask for a [code review][4].


Review code
-----------

A team member other than the author reviews the pull request. They follow 
[Code Review][4] guidelines to avoid miscommunication.

They make comments and ask questions directly on lines of code in the Github web
interface.

For changes which they can make themselves, they check out the branch.

    git checkout <BRANCH-NAME>
    git diff staging/master..HEAD

They make small changes right in the branch, test the feature in browser, run
tests, commit, and push.

When satisfied, they comment on the pull request `Ready to merge.`


Merge
-----

Rebase interactively. Squash commits like "Fix whitespace" into one or a small
number of valuable commit(s). Edit commit messages to reveal intent.

    git fetch origin
    git rebase -i origin/master

View a list of new commits. View changed files. Merge branch into master.

    git log origin/master..<BRANCH-NAME>
    git diff --stat origin/master
    git checkout master
    git merge <BRANCH-NAME> --ff-only
    git push

Delete your remote feature branch.

    git push origin --delete <BRANCH-NAME>

Delete your local feature branch.

    git branch --delete <BRANCH-NAME>


Deploy
------

Yo, use whatever method that [floats your boat][5].

[1]: "http://en.wikipedia.org/wiki/Convention_(norm)"
[2]: http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html
[3]: https://help.github.com/articles/using-pull-requests/
[4]: ../code-review/README.md
[5]: http://en.wiktionary.org/wiki/whatever_floats_your_boat