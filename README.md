# demo2-github
An example for students of BIOS606

Please use this repo to inspect how GitHub and BitBucket present commit history and their associated differences.

Note that this is a Markdown format text file. These are often used for documentation purposes as they allow easy 
text formatting and are rendered nicely by both GitHub and Bitbucket.

To learn more about markdown visit <https://help.github.com/articles/markdown-basics/>.

## First steps
Exploring and comparing [GitHub](https://github.com/bioboot/demo2-github) and [Bitbucket](https://bitbucket.org/bjgrant/demo2-github/).

- Clone this repo with `git clone https://github.com/bioboot/demo2-github.git`
- Browse this repo on the websites of [GitHub](https://github.com/bioboot/demo2-github) and [Bitbucket](https://bitbucket.org/bjgrant/demo2-github/).
- Use your command line knowledge of git to inspect history, contributors and differences.
- Which do you prefer, GitHub or Bitbucket?

## Second steps
Now create your own GitHub account at <https://github.com/> by using your UMICH email and a distinct passwd. Then create your fist GitHub repo by following these instructions:

- In the upper-right corner of any page, click **+** (plus symbol), and then click **New repository**.
- Create a name for your repository. For example, "demo3-github-barry". (**note please replace barry with your unique name!**)
- Optionally, add a description of your repository. For example, "My first repository on GitHub."
- Choose a **public** repository. (Note that these are visible to any user on GitHub, so you can benefit from a collaborative community, but do please keep your content clean! 
- Select **Initialize this repository with a README**.
- Click Create repository.
- You can now edit your README.md file on GitHub or just clone to your machine with `git clone <URL>`


Congratulations! You've successfully created your first repository on GitHub, and initialized it with a _README_ file.

## Third steps
Syncing local and remote repos.

- On your machine cd to your new repo and add some content to the **README.md** file. Also create another file called **ToDo.md** with some items on your to-do list.
- Now add these to your local staging area with `git add README.md ToDo.md`
- Commit these to your local repo (i.e. still on your machine only) with `git commit -m "Edit README.md and add ToDo.md"
- Push these to your **remote** GitHub repo with 'git push -u origin master'

Congratulations! you have just updated your GitHub repo.

## Fourth steps
Collaborating with remote repos.

- Now partner with the person beside you and decide on **ONE repo** that you would like to collaborate on (i.e. the person on the right).
- If you are the owner of this **One repo** add the other person as a collaborator to your GitHub repo.
- Ask for the **username** of the person you're adding as a collaborator. 
- On GitHub, navigate to the main page of the repository.
- In the repository's right sidebar, click  **Settings** (it looks like a little gear icon)
- Click the "**Collaborators**" tab.
- Start typing the collaborator's username.
- Select the user from the drop-down menu.
- Click **Add**.

### Contributing to your partners repo
- If you are the collaborator, clone your partners repo by getting the URL from GitHub (`git clone <URL>`.
- Modify some of the files (for example add some content to the **ToDo.md** file)
- Go through the regular git add/git commit cycle.
- Push these changes to GitHub with `git push -u origin master`

Congratulations! you have now contributed to a shared collaborative repo! 

## Fifth steps
Generating and fixing conflicts.

- Now together with your partner pick a common line and edit it in different ways so you will have two distinct versions.
- First `git pull origin master` to sync with remote repo.
- Then `add/commit/push` your changes to GitHub.
- What happened?

Can you fix your first **conflict**?






