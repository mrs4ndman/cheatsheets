# Git commands

## A collection of the most-used git commands and their submodules / options
## They are ordered in what I believe is their most-common usecase order

### git add

- `\.` : Adds all the files in the working directory to the index
- \<filename\> : Adds the file / directory specified to the index
- `-e` / `--edit` : Opens the diff between the working directory and the index in an editor. After closing, applies the select patch to the index
- `-f` / `--force` : Forces the addition of a file that would otherwise not be added (files affected by .gitignore, for example)
- `-v` / `--verbose` : It represent the action as verbose, providing more information of the actions taken
- `-i` / `--interactive` : Interactive mode: Adds modified contents in the working tree interactively, allowing revision of the modified elements
- `-u` / `--update` : Updates the index for already-tracked files in the entire working directory tree. If given a pathspec / filename, updates it but does not add any new files
- `-p` / `--patch` : Allows you to choose hunks to "patch" the index with
- `-A` / `--all` : Updates already-tracked pathspecs / files to match the working tree

[comment]: # TODO: Complete cheatsheet
### git commit




### git diff

### git revert

### git checkout

### git branch

### git log

### git blame

### git cherry-pick

### git rebase

### git tag

### git stash

### git push

### git pull
