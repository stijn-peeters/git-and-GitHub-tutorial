# How to use git and github

## 1. Follow the verry first tutorial on codeacadamy to understand git

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

## 2. Linking your Git with GitHub
<details>

### The first job is to authenticate your machine in github
<summary>Show me how to link</summary>
You can do this by storing your credentials or creating an SSH key.

#### We will create an SSH key as it is far more secure.

Creating an SSH key depends on the machine (OS) you use.

<details>
<summary>LINUX</summary>
Generate SSH-key (Linux)

1. Open your terminal
2. Copy the following command into your terminal 
    Change "your_email@example.com" to the email address linked to your Github account and press `Enter`.

    ```shell
    ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
    ```

    This will create an SSH key that is linked to your email

3. Generate a private/public RSA key pair
    When you are asked to "Enter a file in which to save the key", press `Enter`. This will accept the standard location.

4. Enter a file in which to save the key (/home/*user_name*/.ssh/id_rsa): [Leave blank and press `Enter`]
5. Enter passphrase (empty for no passphrase): [Leave blank and press `Enter`]
6. Enter same passphrase again: [Leave blank and press `Enter`]

</details>

<details>
<summary>MAC</summary>
Use Github on the terminal (for Mac)

To login into github you need a SSH-key. In the next steps we will see how to generate one and link it to your github account.
Generate a SSH-key (for Mac)

1. Open your terminal
2. Copy the following command into your terminal 
    Change "your_email@example.com" to the email address linked to your Github account and press `Enter`.

    ```shell
    ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
    ```

    This will create an SSH key that is linked to your email
3. Generate a private/public RSA key pair
    When you are asked to "Enter a file in which to save the key", press `Enter`. This will accept the standard location.

4. Enter a file in which to save the key (/Users/*user_name*/.ssh/id_rsa): [Leave blank and press `Enter`]
5. Enter passphrase (empty for no passphrase): [Leave blank and press `Enter`]
6. Enter same passphrase again: [Leave blank and press `Enter`]

</details>

<details>
<summary>WINDOWS</summary>
Use GitHub on the terminal (for Windows)

To login into github you need a SSH-key. In the next steps we will see how to generate one and link it to your github account.
Generate a SSH-key (for Windows)

1. Open you Terminal/cmd.
2. Copy the following command into your terminal 
    Change "your_email@example.com" to the email address linked to your Github account and press `Enter`.

    ```shell
    ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
    ```

    This will create an SSH key that is linked to your email
3. Generate a private/public RSA key pair
    When you are asked to "Enter a file in which to save the key", press `Enter`. This will accept the standard location.

4. Enter a file in which to save the key (/c/Users/*user_name*/.ssh/id_rsa): [Leave blank and press `Enter`]
5. Enter passphrase (empty for no passphrase): [Leave blank and press `Enter`]
6. Enter same passphrase again: [Leave blank and press `Enter`]

</details>

#### Now that we created our SSH-key we can put it in GitHub

First we will copy our SSH-key

- Linux
```xclip -sel clip < ~/.ssh/id_rsa.pub```

- Mac
```pbcopy < ~/.ssh/id_rsa.pub```

- Windows
```clip < ~/.ssh/id_rsa.pub```

Now that our SSH-key is copied we will paste it in GitHub.
![](https://i.imgur.com/A5JTP6P.png)

After you followed the above steps in the image you click "New SSH key".

Then you name your key eg. "pc becode" and paste your key in the second window
![](https://i.imgur.com/oXBHyp0.png)

Finaly click Add key
</details>

###  Now your machine is known in GitHub
<details>
<summary>Testing time!</summary>
Ofcourse we want to know how to ```git push``` something to Github.

First of all we create a folder ```mkdir newfolder``` and we go to it in the terminal ```cd newfolder```

Then we go to the github website.

And we add a new repository to our profile.

![](https://i.imgur.com/aV8gsvS.png)
![](https://i.imgur.com/uGzzeVA.png)

Finaly we copy and paste all the commands as shown below in the image.
![](https://i.imgur.com/aedRrmu.png)

#### If you entered all the commands correctly (and you will have entered the last command push) you will not be asked to log in with your credentials.
</details>

## 3. Import from github to Visual Studio Code

<details>
<summary>How to clone a repository</summary>
1. Create a directory on the local file system.
2. Create a repo on Github.
3. Select Clone "Clone or download" on Github, copy the link

![](https://i.imgur.com/McE8bet.png)

4. In Visual Studio Code, sect File -> Add Folder to Workspace ->Select the newly created directory
5. Select Terminal Window
In the window, type:

```
git config --global user.name <github userID>

git clone <URL from github link copied earlier>
```
</details>

## 4. Problems

"I still need to log in???!!? SSH NOT WORKING"

First

```git remote -v```

If any of your remotes are starting with https you are NOT using your SSH-key

To fix this:

```git remote rm origin```

Re-add the remote location you have added before from github.

```git remote add origin new_link_see_below```

<details>
<summary>when cloning</summary>

![](https://i.imgur.com/McE8bet.png)

</details>

<details>
<summary>when creating a new repository</summary>

![](https://i.imgur.com/aedRrmu.png)

</details>
