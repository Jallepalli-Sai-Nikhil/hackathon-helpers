setup
############################################################################
git --version

git config --global user.name "Your Name"

git config --global user.email "you@example.com"

git config --list

git config --global init.defaultBranch main

git config --global core.editor code

git config --global credential.helper manager




status
########################################################################
git status

git status -s

git diff

git diff --staged

git diff HEAD



staging
###########################################################################
git add .

git add *

git add src/

git add pom.xml

git add -A

git add -u

git add -p



unstage
##############################################################################
git restore --staged file.java

git reset HEAD file.java

git reset





commit
#################################################
git commit -m "Initial Commit"

git commit

git commit -am "Update"

git commit --amend

git commit --amend --no-edit


logs
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
git log

git log --oneline

git log --graph

git log --decorate

git log --all

git log --stat

git log --author="John"

git log --since="2 days ago"

git shortlog



branch
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~`
git log

git log --oneline

git log --graph

git log --decorate

git log --all

git log --stat

git log --author="John"

git log --since="2 days ago"

git shortlog






git push

git push origin main

git push origin feature/user

git push -u origin feature/user

git push --all

git push --tags

git push --force

git push --force-with-lease









