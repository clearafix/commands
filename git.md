#GIT

Delete git tags

```
git tag -l | xargs -n 1 git push --delete origin
``` 

and then delete the local copies: 

```git tag | xargs git tag -d```