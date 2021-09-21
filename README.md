To create a git repository: 


# Method One - Creating local and remote repos separately and then connecting them. 

### Download the exercise file from Frodo
1. Download the project folder from Frodo. You may have to unzip it. 
2. Using the Finder or the File Explorer, drag the project folder where you want it (I suggest having a DevMountain folder with an afternoon-projects folder organized into weeks).
2a. Alternatively, if you are comfortable with the command line you could move the folder using the `mv [file/folder] [destination]` command, where [file/folder] is the item to be moved, and [destination] is the folder you would like to move it to. 
### Set up the local repo
1. In your command line, navigate into the project folder you would like to make a repo in. *You should only create a single repo for a single project*. Type in pwd to make sure you're in the correct place. 
2. `git init` Once you are sure you're in the correct folder, you want to initialize a git repo so that git will track the changes you make in the project. 
3. `git add .` This will add any changes you've made since the last commit. You can also add specific files like so: `git add [filename]`. Git is now tracking those files and any changes you've made to them. 
4. `git commit -m "some commit message"` Now we can save a version of the project by committing it. This takes a snapshot or creates a version of the project that can be referred to at a later date.

Your project is now a local repo and you've tracked and saved the current version. 

### Creating and connecting the remote repo
1. Go to Github and create a new repo. The name should exactly match the name of the local repo folder. (It will work if the names do not match, but typically mismatched names for the local and remote repos leads to confusion.)
2. After creating the repo you'll be presented with a setup page. Copy the commands from the section titled **…or push an existing repository from the command line**. It should have the following commands: 
 - git remote add origin https://github.com/suthyscott/[NAME-OF-YOUR-REPO].git
 - git branch -M main
 - git push -u origin main
3. Paste the commands into your command line *in the folder with your local repo*. On Windows you may have to hit enter to run the last command manually after pasting it. 
4. Go to GitHub and refresh the page. You should now see the changes you made. 

### Once the local and remote repos are connected
As you code and make changes that you want push up, follow the below steps:
1. `git status` *optional* Shows the status of the git repo. Any files in which you've made changes will be listed out, in red. 
2. `git add .` This will add any changes you've made since the last commit. You can also add specific files like so: `git add [filename]`. Git is now tracking those files and any changes you've made to them. 
3. `git status` *optional* You should now see the files you added in green, showing that they're ready to commit. 
4. `git commit -m 'some commit message'` will take a snapshot or save a version of the folder as it currently is. 
5. `git push` After connecting the remote repo, git will have a record of where to push your files. Once you've pushed, you can go and view the changes on GitHub. 



# Method two - creating the repo in GitHub

1.	Go into GitHub
2.	Sign in
3.	Click the green “New” button towards the left corner
4.	Give your repository a name
5.	In the section titled **…or create a new repository on the command line** click the button on the right side to copy that code (Below is the code)
  -	`echo "# test1" >> README.md` - the word “test1” will be your repository name
  - `git init`
  - `git add README.md`
  - `git commit -m "first commit"`
  - `git branch -M main`
  - `git remote add origin https://github.com/adam-hunter13/test1.git` - the word “test1” will be your repository name
  - `git push -u origin main`
6.	Download needed material from DevMountain
7.	Open Finder/File Explorer
8.	Move that download to the folder where you want the final project to be saved at
9.	Open your computer’s terminal
10.	Navigate to where you moved that downloaded file
11.	Once you have made it to the file location type `code .`
12.	This will open that file in VS Code
13.	Navigate back to your computer’s terminal
14.	Paste the code from Step 5
15.	Click back into GitHub and refresh the page
 - You should see that your new repository now has one commit
16.	Begin typing your code within VS Code
17.	When you’ve reached a point where you want to make another commit, click in the VS Code Terminal or your computer’s terminal. Make sure you are in the root folder for the project and type `git add .` This will add any changes you've made since the last commit. You can also add specific files like so: `git add [filename]`. Git is now tracking those files and any changes you've made to them. 
18.	Next we want to create a message for our commit in the terminal type `git commit -m “message”`
19.	Once that code has populated within the terminal you will next type `git push` 
20.	Navigate back to GitHub and refresh the page. You should see that the repository has a new commit with all the code you have created. 


## No matter how you created and connected your local and remote repos: 

### As you code and make changes that you want push up, follow the below steps:
1. `git status` Shows the status of the git repo. Any files in which you've made changes will be listed out, in red. 
2. `git add .` Will add or start tracking any files in which you've made changes. 
3. `git status` Should show the files you've added in green, showing that they're ready to commit. 
4. `git commit -m 'some commit message'` Will take a snapshot or save a version of the folder as it currently is. 
5. `git push` After connecting the remote repo git will have a record of where to push to, so you can just push and then go and view the changes on GitHub. 


## Useful commands:
1. `git remote -v` will show you the URL to the remote repo connected to your local repo, **OR** nothing if the local repo is not connected to any remote repo. 
3. `pwd` not a git command, but very useful in the command line to see what directory/file path you are currently in. 
4. `ls` shows which files and folders are contained in the current directory. 



## Useful notes:
Folder and directory mean the same thing. 

Your command line directly reflects the files and folders in your File Explorer or Finder. 