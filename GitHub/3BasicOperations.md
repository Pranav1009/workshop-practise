
# Hi there!

Now that we have successfully installed and configured GitHub, it's time to actually use it! To begin with, we'll be creating a local copy of your brand new but empty repository, and putting it to more use. Read on, then!

## Forking

One of the primary reasons why people use GitHub is that it enables easy code sharing and collaborative development. One of the most important features of GitHub is the ability to fork an existing repository. 

When you fork a repository, it creates a carbon copy of that repository on your account that you can then modify to your heart's content. You can then request the original maintainer to accept your modifications, which we'll talk about later. 

To fork, we'll be using this same repository! You are going to get your own copies of all these files. 

- Head over to the repository's root directory. (https://github.com/cyberwizard1001/workshop-practise)
- Once you're here, find the button that says 'Fork', and click on it. 
- Voila! You are now the proud owner of a copy of this repository. You can now modify this as you please, as long as you don't violate the license of whoever you're forking from (which doesn't usually happen, as copyrighted code will be in private repositories anyway)


## Cloning

- Now that you have a copy of this repository on your GitHub account, you can download this code and work offline on your desktop/laptop.
- This is called **cloning**.
- To clone a repository, we need a link for the same. Find the ***green* download code button** and click on it. 

### Git CLI:
- Assuming you're using git CLI, we will be using a command to download the code to our local machine. Click on the *notepad* icon next to the repository link inside the download dropdown. This saves the git URL to your clipboard, ready to be pasted. 
- Search for Git CLI in the Start menu on your local machine and click on the Git CLI app. A terminal window should open at this point, pointing to your home directory. 
- Navigate to the directory you want this repo in (using the *cd* command) and run the following command: 

```git clone https://github.com/cyberwizard1001/workshop-practise.git ```

(Paste the downloaded link by right clicking and selecting *paste* or using the Shift+Ins keyboard shortcut or any other pasting shortcut that applies to your system)

Now, press **ENTER**.

And we're done! You should see the files downloading at this point. Once the command is complete, you have an up to date copy of the code that's on your repository on your local machine! 

## Committing

#### Modify a file:
Now that we have a local copy, it is time to make some change and send it to the remote repository. Let's begin by modifying the file ***YourNameHere***.

Navigate to /GitHub and open the YourNameHere file using Notepad / any other code editor. 

Now, add your name to this file, save and exit. We're ready to commit!

#### Committing:
Commits are done to save the state of a repository. Once you have added/removed/modified any files you want to, you need to let Git know that it needs to save the changes at this point. Kind of like pressing Ctrl+S while editing a file. It creates a snapshot of the code at this point. 

- We begin by adding the files to be uploaded to remote using the **git add** command.

	To do so, run the following command: 
	
	``` git add . ```
	
	> The ```.``` here signifies that all files are to be added. You can mention individual filenames as well. Just make sure that no editor created folders are there by deleting them in the local copy.

- To commit the changes that we've done, we use the **git commit** command. 

Command: 

``` git commit -m "My first commit ever"```

The changes are added to the Git system with the commit comment 'My first ever commit ever' ( ```-m``` stands for message).

And just like that, you have made your first commit! 

## Pushing

Okay, so you have an edit on your local system that the remote repository needs to know about. How do we go about telling it?

We do this by running the ```push``` command. It does exactly what the name states, pushing your local changes to the remote. 

To push your changes to the remote copy, run the following command:

```git push```

- When the command completes and exits (assuming there's no error), you have pushed to the repository! Kudos. 
- To verify that the push was successful, head over to the browser, open your repository and check the file structure and last updated time!
- To be absolutely sure, open the YourNameHere file to verify that your name has been added. 


## Pulling

Assume you are working from multiple devices, or that you are collaborating with someone. Your local copy is old, and you want to refresh the repository by downloading the changes. What do you do?

Say hi to Pull.

Simply run the command 

```git pull``` 

and it will download any new changes to your local repository!

### Moving forward: 

And with that, we have covered most of the basics of how to use GitHub. If all you want to do is use GitHub as a place to store your code, you're basically done at this point. But the key purpose of Git is for collaboration (and it will come in REALLY useful in your third semester final projects!) and to collaborate, we're going to learn a couple more things. 

Check out the next file!
