# TASK1.MD

* Go to gitlab.com and create new project using gui button. Choose public option.

* Git was already installed but  

```bash
sudo apt install git #(deb/ubuntu)  
sudo pacman -S git #(arch/manajro)  
dnf install git #(Fedora 22+)  
git-scm.com/download/win #(windows installer link)  
```  

* Initialize local repository

```bash
cd 'your preferred path'
mkdir Git-hw
cd Git-hw
git init
```

* Link local repository to remote (rhw - short name)

```bash
git remote add rhw https://gitlab.com/Gadzillos/git-homework
```

* commit this file to local repository ()

```bash
mv TASK1.MD Git_hw/
```

```bash
git add TASK1.MD
git commit -m "added TASK1.md file"
```

* Push into remote repository

```bash
git branch -M main
git push -u rhw --all
```

* go to gitlab and witness all of yoyr markdown being screwed => go to https://www.markdownguide.org/basic-syntax and learn markdown syntax =(  Good markdown editor - VS code + markdownlint extension  

> The task was successfully completed!:)
