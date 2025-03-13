# Use this commands to use Git

1. Push code to Github

>git remote add origin repo_url

>git branch -M main

>git push -u origin main

To remove origin 
>git remote remove origin

If problem in push
>git pull --rebase origin main

2. clone a Repository

>git clone repo_url

3. Git Ignore commands

This command will ignore all .txt files in repository
> *.txt

This command will ignore all folders named "node_modules"
>node_module

This commands will ignore all png files by not in "screenshots" folder
>*.png

>!/screenshots/*.png