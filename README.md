# Git-Aliases

Cheatsheet for Git aliases

Languages [EN](#en) | [TR](#tr)

## EN

### Overview

This document provides a comprehensive set of Git aliases designed to streamline your workflow by shortening commonly used Git commands. Aliases are shortcuts that allow you to execute commands more efficiently, saving time and reducing the chances of errors.

### Alias List and Descriptions

| Alias | Git Command | Description |
|-------|-------------|-------------|
| `gpl`  | `git pull`  | Fetches and merges changes from the remote repository into the current branch. |
| `gpush`  | `git push`  | Pushes the committed changes from the local repository to the remote repository. |
| `gsta`  | `git status`| Displays the state of the working directory and staging area. |
| `gbr`  | `git branch`| Lists all branches in the repository or creates a new branch. |
| `gco` | `git checkout` | Switches branches or restores working tree files. |
| `gcb` | `git checkout -b` | Creates and switches to a new branch. |
| `gdif`  | `git diff`  | Shows the differences between the working directory and the index. |
| `gadd`  | `git add`   | Adds file contents to the staging area. |
| `gcom` | `git commit`| Records changes to the repository with a message. |
| `greb`  | `git rebase` | Reapplies commits on top of another base tip. Useful for integrating changes. |
| `gmer`  | `git merge`  | Combines multiple sequences of commits into one unified history. |
| `grh` | `git reset HEAD~` | Resets the current HEAD to the specified state, typically used to undo the last commit. |
| `gsta` | `git stash`  | Temporarily stores all modified tracked files. Use `git stash pop` to retrieve them. |
| `glg` | `git log --oneline --graph --all` | Displays a condensed view of the commit history with a graphical representation of branches. |
| `gfa` | `git fetch --all` | Fetches all changes from all remote repositories. |
| `gcl` | `git clone`  | Clones a repository into a new directory. |

### Setting Up Git Aliases

#### For Git Bash, Linux, and macOS Users:

1. **Open your terminal.**
2. **Navigate to your home directory:**
   ```bash
   cd ~
   ```
3. **Open the `.bashrc` or `.bash_profile` file:**
   ```bash
   nano ~/.bashrc
   ```
   or
   ```bash
   nano ~/.bash_profile
   ```
4. **Append the following aliases to the end of the file:**
   ```bash
   alias gpl='git pull'
   alias gpush='git push'
   alias gsta='git status'
   alias gbr='git branch'
   alias gco='git checkout'
   alias gcb='git checkout -b'
   alias gdif='git diff'
   alias gadd='git add'
   alias gcom='git commit'
   alias greb='git rebase'
   alias gmer='git merge'
   alias grh='git reset HEAD~'
   alias gsta='git stash'
   alias glg='git log --oneline --graph --all'
   alias gfa='git fetch --all'
   alias gcl='git clone'
   ```
5. **Save and close the file.**
   - **To save:** Press `Ctrl + O`, then `Enter`
   - **To exit:** Press `Ctrl + X`
6. **Apply the changes by refreshing the shell:**
   ```bash
   source ~/.bashrc
   ```
   or
   ```bash
   source ~/.bash_profile
   ```

#### For Windows PowerShell Users:

1. **Open PowerShell.**
2. **Edit your PowerShell profile file:**
   ```powershell
   notepad $PROFILE
   ```
3. **Add the following alias functions:**
   ```powershell
   function gpl { git pull }
   function gpush { git push }
   function gsta { git status }
   function gbr { git branch }
   function gco { git checkout }
   function gcb { git checkout -b }
   function gdif { git diff }
   function gadd { git add }
   function gcom { git commit }
   function greb { git rebase }
   function gmer { git merge }
   function grh { git reset HEAD~ }
   function gsta { git stash }
   function glg { git log --oneline --graph --all }
   function gfa { git fetch --all }
   function gcl { git clone }
   ```
4. **Save and close the profile file.**
5. **Activate the changes by restarting PowerShell or running:**
   ```powershell
   . $PROFILE
   ```

### Using Git Aliases

Once configured, you can use the aliases in your terminal to streamline your Git workflow.

### Conclusion

Git aliases are powerful shortcuts that help you perform frequent operations more efficiently. By integrating these aliases into your workflow, you can save time and reduce errors, enhancing your productivity in managing Git repositories.

