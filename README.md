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
git add * // if new files
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


#### Merge branch into another

```shell
// On the branch that you want to merge with, the neglect branch
git merge (target_branch_name)
git checkout (target_branch_name)
git merge (neglect_branch_name)
```


#### Get repo status

```shell
git status
```


#### Create tag to commit

```shell
git tag (tag_name) (commit_id)
```


#### Get repo log

```shell
git log
```
