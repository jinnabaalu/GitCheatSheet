# Ops Commands

- **Recursively remove all untracked files in the tree.**
  - Command: `git clean -f`

- **Throw out all of your changes to existing files, but not new ones.**
  - Command: `git reset --hard`

- **Remove file from staging area.**
  - Command: `git rm --cached [file]`

- **See diff of files in the staging area.**
  - Command: `git diff --staged`

- **See tracked files.**
  - Command: `git ls-files`

- **See a branch graph.**
  - Command: `git log --graph`

- **See all tags.**
  - Command: `git tag`

- **See a list of deleted files.**
  - Command: `git ls-files -d`

- **Restore all deleted files.**
  - Command: `git ls-files -d | xargs git checkout --`

- **View commits not yet pushed to remote.**
  - Command: `git log --branches --not --remotes`

- **Difference between two branches.**
  - Command: `git diff --stat --color master..branch`

- **See a list of all objects.**
  - Command: `git rev-list --objects --all`

- **Remove file from index.**
  - Command: `git rm --cached filename.txt`

- **Get a list of all commit messages for a repo.**
  - Command: `git log --pretty=format:'%s'`
