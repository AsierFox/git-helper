# git helper

#### Create a repository

```shell
git init
```


#### Clone repository

```shell
git clone (url)
git clone (username)@(host):(/path/to/repo)
```


#### Push changes to branch

```shell
git add * # if new files
git commit -m "(commit_message)"
git push origin (branch)
```


#### Pull from server (update)

```shell
git pull
```


#### Create a branch

```shell
git checkout -b (branch)
```


#### Switch to another branch

```shell
git checkout (branch)
```


#### Sync master with develop
```shell
# Merge master into develop (Fire command from master branch, due to is AHEAD)
git checkout master
git merge develop
# Merge develop to master
git checkout develop
git merge master
```


#### Merge branch into another

```shell
# On the branch that you want to merge with, the neglect branch
git checkout (target_branch_name)
git pull origin (target_branch_name)
git merge --no-ff (neglect_branch_name) # No fast forward (To not lose commits)
git push origin (target_branch_name)
git checkout (neglect_branch_name) # Return to neglet branch
```

```shell
# merge develop into master (Fire command from develop branch)
git checkout master && git pull origin master && git merge --no-ff -m "merge develop to master" develop && git push origin master && git checkout develop
```

#### Change remote from Bitbucket repository to Github

```shell
git remote rename origin bitbucket
git remote add origin <url_github_repo>
git push origin master

git remote rm bitbucket
```


#### Get repo status

```shell
git status
```


#### Undo/Remove commit

```shell
git revert -m "revert commit (description)" (commit_id)
```


#### Create tag to commit

```shell
git tag (tag_name) (commit_id)
```


#### Get repo log (All commits history)

```shell
git log
```
