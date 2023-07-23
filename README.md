# WITSOC X UCIEEE git workshop

Group repository for the WitSoc and UCIEEE git workshop at the University of Canterbury.

Welcome to the group repo for the git workshop!

The goal for today is to successfully get a file (not specifically code, unless you want!) from each of the other people here onto your computer.

This demonstrates the power of git and exemplifies how easy it is for group work, saving your files securely and accessing your code on any computer.

### Step One: Create a folder and open the Terminal
Create a folder called `git workshop` or similar somewhere you will find it.

Right click on the folder and select `Open in Terminal`.

### Step Two: Clone the repository
Click the blue drop down menu that says `Code` in the top right hand corner of the page. 

Copy the HTTP link.

Go to the Terminal and type `git clone {link you cloned}`

A folder should be created called `git-workshop`.

### Step Three: Create a new document
Create a document, call it anything you want - ideally something unique so there are no double ups!

You can put anything you want in it, it can be a text file, python file, Java file or even an image.

Make sure to save it into the `git-workshop` folder.

### Step Four: Add the file to git
Now back to the Terminal:
- Enter the command `git status` you should see something along the lines and the filename should be red:
```
Untracked files:
  (use "git add <file>..." to include in what will be committed)
	Test.docx
```
"[Untracked] basically means Git is aware the file exists, but still hasn't saved it in its internal database" - https://www.cloudbees.com/blog/git-remove-untracked-files 

- Enter the command `git add <file name>`, this adds the new file to the staging area and means that the git will now track the file.
- If you re-enter `git status` you will notice that your file is now tracked. This means it is ready to be committed and then pushed to the remote repository where we will be able to find it on GitLab!

The output should now look like below and the file name is green:
```
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	new file:   Test.docx
```

### Step Five: Commit your changes and push to the remote repository.
Now that you have added your files to git, we will commit and push them to our group repo so that everyone can see them.

To commit changes enter the command: 
`git commit -m "<Add a relevant message in here that describes any changes you made, but for now it can be anything>"`

The `-m` means you are going to add a message, it's always necessary to add a message especially when you are working in a team so everyone can see what changes have been made.

Next we are going to push these changes to the remote repository so your neighbours can see the changes you made!

To do this enter the command: 

`git push`

GitLab will require you to log in when you first push your changes, so enter the email and password you created your account with and it should be good to go!

### Step Six: See your changes here

Now you can go to the sidebar and open the `Repository` tab. 

Your file should be there **and** your commit will be too. 

The best thing about git is you can view code base history and track any changes made by anyone.

### Step Seven: See other peoples changes on your computer
Once others have pushed files to GitLab we will be able to **pull** these changes and see them locally.

To do this we simply execute: `git pull`

This will update the directory with the changes and you will be able to see the new files on your lab computer. 

### Done!
So that is us all done for the tutorial now, if you've finished early check out these links or feel free to start creating repositories for your different classes and adding your files to them: 

[Atlassian Article on git](https://www.atlassian.com/git/tutorials/what-is-git)\
[Git Branching- useful for a project with many features](https://www.educative.io/blog/git-branching-tutorial)

You can also use git in an IDE like Intellij or VSCode instead of using the Terminal (unfortunately not Wing).
