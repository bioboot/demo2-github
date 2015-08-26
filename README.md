# GitHub Demo2 
An example for students of [biocomputing bootcamp BIOS606](http://bioboot.github.io/web-2015/)

We will first use this repo to inspect how GitHub and BitBucket present commit history and their associated differences. Then we will explore different way to colloborate with others through the GitHub version of this repo.

Note that this is a Markdown format text file. These are often used for documentation purposes as they allow easy 
text formatting and are rendered nicely by both GitHub and Bitbucket.

To learn more about markdown on your own time visit <https://help.github.com/articles/markdown-basics/>.

For this second GitHub demo (hands-on exercise) please complete the steps below and remember to please feel free to talk to your neighbors and ask questions as you go: 

## 1. Exploring and comparing [GitHub](https://github.com/bioboot/demo2-github) and [Bitbucket](https://bitbucket.org/bjgrant/demo2-github/).
- In your terminal first make sure you are in a suitable working directory, e.g. `~/Desktop/git_class`
- Clone this repo with `git clone https://github.com/bioboot/demo2-github.git`
- Then `cd demo2-github/` and use your command line knowledge of git to inspect history (`git log`), contributors and differences.
- Now browse the two online version of this same repo on the websites of [GitHub](https://github.com/bioboot/demo2-github) and [Bitbucket](https://bitbucket.org/bjgrant/demo2-github/).
- Which do you prefer, GitHub or Bitbucket?



## 2.  Exploring Pull requests
There are two basic models for collaborating on GitHub and BitBucket. These are known as the **Shared repository model** and the **Fork & pull model** (often just refered to as **Pull requests**).


1. The **shared repository model** is more prevalent with small teams and organizations collaborating on private projects. Everyone is granted **push** access to a single shared repository and different branches are primirarly used to isolate major changes whilst small changes typically get pushed directely to the default **master** branch as you have already done in **demo1**.


2. The **fork & pull model** lets anyone fork an existing repository and push changes to their personal fork without requiring access be granted to the source repository. The changes must then be pulled into the source repository by the project maintainer. This model reduces the amount of friction for new contributors and is very popular with open source projects because it allows people to work independently without upfront coordination.


Here we will explore the *fork & pull** approach as it can be used with any public repo on GitHub or Bitbucket.
- You already have a cone of this repo on your local macine from step one above that you can modify locally and also **pull** updates from.
- However, you don't have permissions to **push** your changes to this origional GitHub repo. Go ahead and try...
- On your local machine (i.e. laptop) open the JustOneThing.md file and add your first name in bold (i.e. surrounded by two starts on either side) and one thing that was not completely clear from todays class thus far (e.g. "staging area").
- Now submit a pull request.
- sentence What happes if You can of course modify away on this local 'sandboxed' copy

Collaborating with remote repos.

- Now partner with the person beside you and decide on **ONE repo** that you would like to collaborate on (i.e. the person on the right).

#### If you are owner of this **One repo**
- Add the other person as a collaborator to your GitHub repo.
- Ask for the **username** of the person you're adding as a collaborator. 
- On GitHub, navigate to the main page of the repository.
- In the repository's right sidebar, click  **Settings** (it looks like a little gear icon)
- Click the "**Collaborators**" tab.
- Start typing the collaborator's username.
- Select the user from the drop-down menu.
- Click **Add**.

#### If you are the collaborator to this repo
- Clone your partners repo by getting the URL from your partners GitHub page (`git clone <URL>`).
- Modify some of the files (for example add some content to the **ToDo.md** file)
- Go through the regular git add/git commit cycle.
- Push these changes to GitHub with `git push -u origin master`

Congratulations! you have now contributed to a shared collaborative repo! 

## 5. Fixing conflicts

- Now together with your partner pick a common line and edit it in different ways so you will have two distinct versions.
- First `git pull origin master` to sync with remote repo.
- Then `add/commit/push` your changes to GitHub.
- What happened?

Can you fix your first **conflict**?






