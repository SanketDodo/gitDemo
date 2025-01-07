# gitDemo

# GIT CHEETSHEET

git config --global user.name "Your Name"        # Set your Git username
git config --global user.email "you@example.com" # Set your Git email
git config --list                                # View your Git configuration


git init                                        # Initialize a new Git repository
git clone <repository-url>                      # Clone an existing repository

git status                                      # Check the current status of your repository

git add <file>                                  # Stage a specific file
git add .                                       # Stage all changes
git reset <file>                                # Unstage a specific file

git commit -m "Commit message"                 # Commit staged changes with a message
git commit --amend                             # Modify the last commit

git branch                                      # List all branches
git branch <branch-name>                        # Create a new branch
git checkout <branch-name>                      # Switch to an existing branch
git checkout -b <branch-name>                   # Create and switch to a new branch
git branch -d <branch-name>                     # Delete a branch safely
git branch -D <branch-name>                     # Force delete a branch

git merge <branch-name>                         # Merge a branch into the current branch
git rebase <branch-name>                        # Rebase the current branch onto another branch

git diff                                        # View changes in the working directory
git diff --staged                               # View changes staged for commit
git log                                         # View commit history
git log --oneline                               # Compact commit history
git log --oneline --graph --all                 # Visualize branch structure
git show <commit-hash>                          # Show details of a specific commit

git stash                                       # Save changes without committing
git stash list                                  # View all stashed changes
git stash apply                                 # Apply the latest stash
git stash drop                                  # Remove a specific stash
git stash clear                                 # Remove all stashes

git remote add origin <repository-url>          # Add a remote repository
git remote -v                                   # View remote repositories
git fetch                                       # Fetch changes from a remote repository
git pull                                        # Fetch and merge changes from a remote branch
git push origin <branch-name>                   # Push changes to a remote branch
git push origin --tags                          # Push all tags to the remote

git checkout -- <file>                          # Discard changes in the working directory
git reset --soft <commit-hash>                  # Reset to a commit, keep changes staged
git reset --mixed <commit-hash>                 # Reset to a commit, keep changes in the working directory
git reset --hard <commit-hash>                  # Reset to a commit, discard all changes
git revert <commit-hash>                        # Create a new commit to undo a specific commit

git tag <tag-name>                              # Create a tag
git tag                                         # List all tags
git push origin <tag-name>                      # Push a specific tag
git push origin --tags                          # Push all tags
git tag -d <tag-name>                           # Delete a local tag
git push origin --delete <tag-name>             # Delete a remote tag


#Cleaning Up

git clean -f                                    # Remove untracked files
git clean -fd                                   # Remove untracked files and directories

#Advanced Commands

git rebase -i <commit-hash>                     # Squash or edit commits interactively
git bisect                                      # Find the commit that introduced a bug
git cherry-pick <commit-hash>                   # Apply a specific commit from another branch