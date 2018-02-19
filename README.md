# gitflow-scripts
Scripts for gitflow

``` Installation for linux
git clone https://github.com/chuhaienko/gitflow-scripts
mkdir -p ~/.local/bin/
cp gitflow-scripts/* ~/.local/bin/
```

### gf-develop
```
gf-develop
```

Reset to actual *develop*.


### gf-master
```
gf-master
```

Reset to actual *master*.


### gf-reset
```
gf-reset
```

Reset to actual current branch.


### gf-check-feature
```
gf-check-feature BRANCH_NAME
```

Differences between actual *develop* and *origin/feature/BRANCH_NAME*.


### gf-check-hotfix
```
gf-check-hotifx BRANCH_NAME
```

Differences between actual *master* and *origin/hotfix/BRANCH_NAME*.


### gf-check-branch
```
gf-check-branch BRANCH_NAME
```

Differences between actual current branch and *origin/BRANCH_NAME*.


### gf-create-release
```
gf-create-release VERSION
```

Create branch *release/FOLDERNAME_VERSION* from actual *master*.
Merge actual *develop* to it.
Push it to remote repository.
*FOLDERNAME* - name of local folder-root of git-repository. 


### gf-after-release
```
gf-after-release
```

Remove branches deleted from remote repository.
Merge actual *master* to actual *develop* and push *develop*.
