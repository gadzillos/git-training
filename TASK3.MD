# TASK3.MD

* Switch to main branch

```bash
git status
git checkout main
```

* modify TASK2.MD

```bash
echo -e '\n> PS I Will do task 3' >> TASK2.MD
git status
```

* add changes to Staging Area

```bash
git add TASK2.MD
```

* use git stash

```bash
git stash
git stash list
# stash@{0}: WIP on main: db27870 Added steps to TASK2.md
git status
```

* Switch to develop

```bash
git checkout develop
```

* Verify that TASK2.md doesn't contain any changes

```bash
git diff TASK2.md
git status
```
* add TASK3.MD with changelog

```bash
touch TASK3.MD
code TASK3.MD 
```

* commit changes

```bash
git add TASK3.MD
git commit -m "added TASK3.MD"
```