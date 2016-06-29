## Delete all branches except develop and master
git branch |grep "develop" | grep "master" | xargs git branch -D

## Add a tag
git tag -a 1.2 -m "Version 1.0"

## Push tags
git push --tags

## Undo a recent commit
git reset --soft HEAD~1
