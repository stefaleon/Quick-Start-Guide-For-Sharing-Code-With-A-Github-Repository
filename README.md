&nbsp;
Problem: You have code you want to share with others and you don’t know git…

&nbsp;
Solution: Here are the basic steps to follow

&nbsp;

1 Install git globally

```
npm i git -g
```

2 In the root folder of your project create a file named _.gitignore_

Include inside it the folders and files that you do NOT want to share.

e.g.

```
node_modules
client/node_modules
config/default.json
private/my_secret_passwords.txt
```

3 Initiate a git repository by typing

```
git init
```

in the console

4 Stage all the files you are about to commit by typing

```
git add .
```

5 Make the commit

```
git commit -m 'YOUR_DESCRIPTIVE_MESSAGE'
```

_YOUR_DESCRIPTIVE_MESSAGE is just informative text_

&nbsp;
So far you have commited your code to a local git repository.
&nbsp;
Now you need to make it public, with a remote repository hosted in Github.
(There are Github alternatives, this is beyond the current scope…)

&nbsp;

6 Sign up and sign in to Github.

7 From the top-right select the + sign , New Repository

8 Set a name for the new repository, e.g myrepo

9 In the next screen, copy the lines from the paragraph
…or push an existing repository from the command line

![image](https://i.imgur.com/vKYdAfs.jpg)

e.g.

```
git remote add origin https://github.com/your_github_name/myrepo.git
git push -u origin master
```

10 Paste those lines in the console and enter

&nbsp;

Now the contents of your project (except the .gitignore includes) are uploaded to a repository in Github which you can share via the url like
https://github.com/your_github_name/myrepo

&nbsp;

![thats all folks!](https://miro.medium.com/max/1400/0*f1vWEOzBr0sdF7Ip.jpg)

&nbsp;
&nbsp;

After on, if you update your code you can be updating your local commits with

```
git add .
git commit -m 'YOUR_NEW_COMMIT_MESSAGE"
```

and also updating the remote copy of your repository in Github with

```
git push
```
