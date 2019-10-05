# Testing the new layout

## Follow the verry first tutorial on codeacadamy

<https://www.codecademy.com/learn/learn-git/modules/learn-git-git-workflow-u>

Follow the first bit of steps that explain the basics of git.

### step 1

Create a folder with terminal or with an interface.
Cd into that folder you just made with terminal and follow the next step.

![](https://i.imgur.com/Jr1cdlz.png)

### step 2


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
