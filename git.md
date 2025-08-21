# Git application notes

## Getting started with git

To get started with git only a few commands are required.
The first command is to initialize your folder with git.

```bash title="initialize your folder with git"
cd source-folder
git init
```

saving add updated files/changes

```bash title="add progress/updates to repository"
git add .          # default: add all changes
git add index.html # add one specific file
```

commiting the updated files/changes to the repository
with a message for more details

```bash title="commit /updates to repository"
git commit -m 'resolved stupid bug in index.html'
```

remove files

```bash title="remove file and commit updates"
rm index.html
git add .
git commit -m 'deleted index.html'
```

look up the update history

```bash title="show update history"
git log
```

revert to previous update / files
use the command below with the HASH code that is shown in the update history

```bash title="show update history"
git checkout 28376418egfdac3428 #HASH code show in the update history
```

## Github

Github are websites where you can put your updates
