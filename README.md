# Git-Command-Lines
A list of useful Git command lines 

### Install Git on Mac 
- Check the current version of Git: ```git --version```
- Configure Git via registering your credentials to Git
	- Add GitLab/GitHub username: 
```git config --global user.name "my_username"```

	- Add email address: 
```git config --global user.email "my_email_address@example.com"```

	- Verify the configuration
``` git config --global --list```



### Clone a repository
- Clone a repo via SSH 
- Clone a repos via https 

- View remote repositories 
``` git remote -v ```

- Download the latest chnges in the current project
```git pull <REMOTE> <name-of-branch>```

### Branches 
- Create a branch 
```git checkout -b <name-of-branch>```

- Switch to a branch 
```git checkout <name-of-branch>```

- View differences 
```git diff```

- View the files that have changes 
```git status```

- Add and commit local changes: 

When you type git status, locally changed files are shown in red. These changes may be new, modified, or deleted files or folders.

1. To stage a file for commit: ```git add <file-name OR folder-name>```

2. Repeat step 1 for each file or folder you want to add. Or, to stage all files in the current directory and subdirectory, type ```git add ..```

3. Confirm that the files have been added to staging: ```git status```. The files should be displayed in green text.

4. To commit the staged files: ```git commit -m "COMMENT TO DESCRIBE THE INTENTION OF THE COMMIT"```


Stage and commit all changes

As a shortcut, you can add all local changes to staging and commit them with one command:

```git commit -a -m "COMMENT TO DESCRIBE THE INTENTION OF THE COMMIT"```

- Send changes to GitLab.com: 
	- To push all local changes to the remote repository: ```git push <remote> <name-of-branch>```
	- Example, push your local commits to the main branch of the origin remote: ```git push origin main```

- Delete all changes in the branch
	- To discard all changes to tracked files: ```git checkout .`` This action removes changes to files, not the files themselves



