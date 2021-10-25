# TASK2.md

* Rewrite your file with vim or VS code. Add steps 7-8 and save it.

```bash
vim TASK1.md
:wq

code TASK1.md

```

* Check the difference

```bash
git status
git diff
```

* commit changes

```bash
git add TASK1.MD 
git status
git commit -m "Rewrited TASK1.md using proper markdown and added steps 7-8"
```

* push into to the remote repository

```bash
git push -u rhw --all
```

* Create `develop` branch and add TASK2.md

```bash
git branch develop
git checkout develop
git status
touch TASK2.md
```

* commit and push to remote

```bash
git commit -m "created develop brach and added TASK2.md"
git push -u rhw develop
```

* modify TASK1.MD

```bash
echo -e '\n> Mission failed!:(' >> TASK1.MD
```

* add, commit and push

```bash
git add TASK1.MD
git commit -m "added a string"
git push -u rhw develop
```

* swith to main branch

```bash
git checkout main
```

* add string to TASK1.MD. commint and push to remote

```bash
echo -e '\n> The task was successfully completed!:)' >> TASK1.MD
git add TASK1.MD 
git commit -m "added a success string"
git push -u rhw main
```

* Try to merge

```bash
git merge develop
Auto-merging TASK1.MD
CONFLICT (content): Merge conflict in TASK1.MD
Automatic merge failed; fix conflicts and then commit the result.
```

* Open TASK1.MD. Delete the conflict markers <<<<<<<, =======, >>>>>>> and make the changes you want in the final merge

```bash
git add .
git commit -m "Resolved merge conflict by keeping main branch string in TASK1.md"
git merge --continue # second option
git push -u rhw main
```

* Check changelog

```bash
git log
```

* commit and push this TASK2.md file

```bash
git add TASK2.md
git commit -m "Added steps to TASK2.md"
git push -u rhw main
```

> PS I Will do task 3
