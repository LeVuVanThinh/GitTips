## Delete all branches except develop and master
git branch |grep "develop" | grep "master" | xargs git branch -D

## Add a tag
git tag -a 1.2 -m "Version 1.0"

## Push tags
git push --tags

## Undo a recent commit
git reset --soft <commit you want to undo>

## Remove local commit
git rebase -i
delete commit you want to delete.

## Remove remote commit
Remove local commit
git push origin +develop (git push origin develop --force)
// Remember that you can't push --force to develop or master by default unless 'master' of repo
