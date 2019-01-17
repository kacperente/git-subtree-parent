**Start with subtree:**
```
git remote add  <name> <url> - add subt**ree url to remotes in parent repo
```
```
git subtree add —-prefix=<name>/ my-subtree master
```
add prefix to subtree, (prefix - subtree directory in parent repo)

**Changing subproject from parent:**
```
git add <file/s>
```
```
git commit -m “<msg>”
```
```
git push <repo> <branch>
```

**Get changes from subproject to parent:**
```
git subtree pull --prefix=<name> —squash <subtree> <branch>
```

**Push changes from subproject in parent to subproject:**
```
git add <file/s>
```
```
git commit -m “<msg>”
```
```
git subtree push --prefix=<name> <subtree> <branch>
```

**Checkout to subproject's tag in parent repo**
```
git subtree pull --squash --prefix=<name> <subtree> tags/<tag>
```