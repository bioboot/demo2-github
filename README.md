# GitHub Demo2 
This is an example for students of [Biocomputing Bootcamp](http://bioboot.github.io/web-2015/) BIOS606 2015

## Overview
We will first use this repo to inspect how GitHub and BitBucket present commit history and their associated differences. Then we will explore different way to collaborate with others through the GitHub version of this repo.

> Note that this README.md file was written as a Markdown format text file. These are often used for documentation purposes as they allow easy text formatting and are rendered nicely by both GitHub and Bitbucket. To learn more about markdown on your own time visit <https://guides.github.com/features/mastering-markdown/> and  <https://help.github.com/articles/markdown-basics/>.

## Directions
For this second _hands-on_ GitHub demo please complete the steps in each of the 3 sections below and remember to feel free to talk to your neighbors and ask questions as you go: 


### 1. Exploring and comparing [GitHub](https://github.com/bioboot/demo2-github) and [Bitbucket](https://bitbucket.org/bjgrant/demo2-github/).
- In your terminal first make sure you are in a suitable working directory, e.g. ` cd ~/Desktop/git_class`
- Clone this repo with `git clone https://github.com/bioboot/demo2-github.git`
- Then `cd demo2-github/` and use your command line knowledge of git to inspect history (`git log`), contributors (`git blame') and differences ('git diff`).
- Now browse the two online version of this same repo on the websites of [GitHub](https://github.com/bioboot/demo2-github) and [Bitbucket](https://bitbucket.org/bjgrant/demo2-github/).
- Which do you prefer, GitHub or Bitbucket?



### 2.  Collaborating on GitHub and BitBucket
There are two basic models for collaborating on GitHub and BitBucket. These are known as the **Shared repository model** and the **Fork & pull model** (often just referred to as **Pull requests**).


1. The **shared repository model** is more prevalent with small teams and organizations collaborating on private projects. Everyone is granted **push** access to a single shared repository and different branches are primarily used to isolate major changes whilst small changes typically get pushed directly to the default **master** branch as you have already done in **demo1**.


2. The **fork & pull model** lets anyone fork an existing repository and push changes to their personal fork without requiring access be granted to the source repository. The changes must then be pulled into the source repository by the project maintainer. This model reduces the amount of friction for new contributors and is very popular with open source projects because it allows people to work independently without upfront coordination.


Below we will explore the **fork & pull** approach as it can be used with any public repo on GitHub or Bitbucket.

> You already have a cone of this repo on your local machine from step one above that you can modify locally and also use `git pull origin master` to sync with any subsequent changes in the original GitHub repo. **However, you don't have permissions to actually `push` your changes to this original GitHub repo**. Go ahead and try if you like… 

Side-Note: If you were added as a 'collaborator' on the repo then you would be able to **git push origin master**, in the same way you did for your own repo in demo1, and contribute your changes directly. This is simply the **shared repository model** and you can create your own by adding 'collaborators' to your own GitHub repos under the *Settings* link. For now we focus on the more complicated **fork and pull** approach. 



## 3. Fork and pull
To get your changes incorporated into someone else's repo that you are not a *collaborator* on requires us to first **fork** the original repo, then **clone it**, make and commit your changes and finally submit something called a **pull request**.

Like many things in the computing world this sounds more complicated than it really is so lets start by **forking** this repo, which basically creates a completely separate copy of the repo under **YOUR** GitHub account.

- To do this click the **Fork** button towards the top right of THIS original GitHub repo 
![img1](https://help.github.com/assets/images/help/repository/fork_button.jpg)

- Now after a short time you should be taken to a new webpage displaying your OWN fork (i.e. your personal copy) of the repo.
- We will now clone this forked repo to your local computer by using the link provided from clicking the somewhat obscure **copy icon** (see image below for an example of the clipboard like icon GitHub like to use).

![im2](https://help.github.com/assets/images/help/repository/clone-repo-clone-url-button.png)

-  When cloning on your computer this time we will add a different destination name **myForkedCopy** after the http address so as we don’t get confused by the repo from step one above. For example:

	git clone https://github.com/YOUR-USERNAME/demo2-github.git myForkedCopy

- Now, you have a local clone of the forked repo on your computer in a new directory named **myForkedCopy**.
- Lets cd into this directory and edit the file **JustOneThing.md** with nano or other means to add your name and a comment (see below). 

	cd myForkedCopy
	echo “**Barry**:  Git and GitHub has a step learning curve” >> JustOneThing.md

For example, add your first name in bold (i.e. surrounded by two starts on either side) and one thing that was not completely clear from todays class thus far (e.g. "staging area", "remote repos" or "where is the coffee?").


- Once you have edited your file in nano go through the regular **git add/commit/push** steps, e.g.

	git add JustOneThing.md
	git commit -m “Edit in my fork of JustOneThing.md"
	git push origin master

- Check that your changes are on-line in YOUR GitHub forked copy.
- Now go to the **pull requests** link on the right hand side
- Click the **New pull request** green button
- It should say *These branches can be automatically merged*
- Add a message such as “Eva's changes from fork” and click **Create pull request** button.


Your changes have been sent to the package maintainer so put your hand up and let me know you have done this so I can demo merging your pull request on the projector for the class.

Congratulations! You have just contributed to this open source project ;)





