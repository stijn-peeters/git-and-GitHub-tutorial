# How to use git and github

## Follow the verry first tutorial on codeacadamy to understand git

<https://www.codecademy.com/learn/learn-git/modules/learn-git-git-workflow-u>


<details>
<summary>In case you already used the free codecademy PRO trial (click arrow)</summary>

### step 1

Create a folder with terminal or with an interface.
Cd into that folder you just made with terminal and follow the next step.


### step 2 

![](https://i.imgur.com/Jr1cdlz.png)

### step 3 
We need some files inside this folder.

You can use ``` echo "GIT exercise" > readme.md ```

### step 4
Now that we made the folder and files we can check our current status.

Checking current folder status

![](https://i.imgur.com/CEL6LGB.png)

Codecademy uses 2 files init_test.rb and scene-1.txt If you followed the previous step you should only see readme.md

### step 5
Git now needs to know what to stage, we will use ```git add``` for this.

For this exercise we will add our readme.md file.

![](https://i.imgur.com/Rv6P6NP.png)

### step 6 (How git works)
![](https://i.imgur.com/L4N4f2X.png)

### step 7
Git can be used in the terminal to see the changes in files after you added them with ```git add```.

The command you can use to see the changes made is ```git diff (filename)```.

![](https://i.imgur.com/ZQ6m2ii.png)

In this example you can see I echoed a new text inside of the readme.md file.

Dont forget to run ```git add``` after you changed the file.

### step 8
Now we can commit to the repository.

![](https://i.imgur.com/bWJ1ds3.png)

The command we use for commit is ```git commit```

Commiting the files you added is building a history for the file, to make searching for changes easier you should add a message (-m).

And in the terminal you cannot use spaces so thats why we will enclose our message(-m) with quotes "just like this".

### step 9
Now we can finaly check if we done all the work correctly.

We will use ```git log``` for this.

>In the output, notice:
>
>    * A 40-character code, called a SHA, that uniquely identifies the commit. This appears in orange text.
>
>    * The commit author (you!)
>
>    * The date and time of the commit
>
>    * The commit message

### with all these commands you should understand the basics of how git works

</details>

Follow the first tutorial that explains the basic workflow of git.

![new account readme](https://i.imgur.com/ijwAd89.png)

## Create a new repository on the command line

```
echo "# new-account" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/stijn-peeters/new-account.git
git push -u origin master
```

## Push an existing repository from the command line

```
git remote add origin https://github.com/stijn-peeters/new-account.git
git push -u origin master
```



## Import from github

1. Create a directory on the local file system.
2. Create a repo on Github.
3. Select Clone "Clone or download" on Github, copy the link
4. In Visual Studio Code, sect File -> Add Folder to Workspace ->Select the newly created directory
5. Select Terminal Window
In the window, type:

```
git config --global user.name <github userID>

git clone <URL from github link copied earlier>
```
<http://www.notyourdadsit.com/blog/2018/4/3/cheatsheet-setup-github-on-visual-studio-code>
