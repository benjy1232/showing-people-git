# This is a readme

This has some text

```
Now some code
```

```py
def some_actual_code():
    print('hello world')
```

To setup SSH key with github:
- `ssh-keygen -t ed25519 -C <comment>` - generates an ssh key of type ed25519 and a comment
- `notepad.exe $HOME\.ssh\id_ed25519` - copy this
- go to github and hit profile picture
- go to Your Preferences
- SSH keys
- Add new one
- paste the stuff you copied
- `ssh -T git@github` - make sure you see your username 

Actual git commands:
- `git config --global user.name <your name>`
- `git config --global user.email <your email>`
- `git init` - Initializes a new git repository in the current folder
- `git status` - checks the status of all your files and if you need to add/remove them
- `git add <filenames>` - Adds whatever files you want to be tracked by git
- `git commit -m <message>` - Commits whatever message you want
- `git push -u origin <branch-name>` - pushes branch to origin
- `git push` - pushes changes to github/bitbucket/whatever you're using
- `git fetch --prune` - updates all the remote branches so think origin/master
- `git pull` - pulls latest changes that are on github/bitbucket/whatever you're using to your computer
- `git checkout -b <branch-name>` - creates a branch of specified name and moves you to working on that branch