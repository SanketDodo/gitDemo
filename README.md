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
