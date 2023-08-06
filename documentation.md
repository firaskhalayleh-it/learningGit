
1. Clone the remote repository:

```bash
firas@firas-GL65-Leopard-10SCSR:~/Documents$ git clone https://github.com/eficode-academy/git-katas.git
```

2. Move into the cloned repository:

```bash
firas@firas-GL65-Leopard-10SCSR:~/Documents$ cd git-katas/
```

3. Create a new branch called "feature/uppercase" and switch to it:

```bash
firas@firas-GL65-Leopard-10SCSR:~/Documents/git-katas$ git checkout -b feature/uppercase
```

4. Create a new file "greeting.txt" and add it to the staging area:

```bash
firas@firas-GL65-Leopard-10SCSR:~/Documents/git-katas$ touch greeting.txt
firas@firas-GL65-Leopard-10SCSR:~/Documents/git-katas$ git add greeting.txt
```

5. Commit the changes to the "feature/uppercase" branch:

```bash
firas@firas-GL65-Leopard-10SCSR:~/Documents/git-katas$ git commit -m "Adding greeting.txt to the repository"
```

6. Edit the "greeting.txt" file to contain an uppercase greeting:

```bash
firas@firas-GL65-Leopard-10SCSR:~/Documents/git-katas$ vim greeting.txt
```

7. Commit the changes again:

```bash
firas@firas-GL65-Leopard-10SCSR:~/Documents/git-katas$ git commit -am "Modify greeting.txt to have an uppercase greeting"
```

8. Switch to the "master" branch:

```bash
firas@firas-GL65-Leopard-10SCSR:~/Documents/git-katas$ git checkout master
```

9. Merge the changes from the "feature/uppercase" branch into the "master" branch:

```bash
firas@firas-GL65-Leopard-10SCSR:~/Documents/git-katas$ git merge feature/uppercase
```

10. View the contents of the "greeting.txt" file after the merge:

```bash
firas@firas-GL65-Leopard-10SCSR:~/Documents/git-katas$ cat greeting.txt
```

11. Push the changes to the remote repository:

```bash
firas@firas-GL65-Leopard-10SCSR:~/Documents/git-katas$ git push origin master
```

## note:
for sure i used the command 
```bash
git remote add origin https://github.com/firaskhalayleh-it/learningGit.git
```
then use the 11'th step

# the second exercise :

```bash
# Step 1: Set up the repository
firas@firas-GL65-Leopard-10SCSR:~/Documents/git-katas/ff-merge$ source setup.sh

# Step 2: Examine the current status and commit history
firas@firas-GL65-Leopard-10SCSR:~/Documents/git-katas/ff-merge/exercise$ git status
firas@firas-GL65-Leopard-10SCSR:~/Documents/git-katas/ff-merge/exercise$ git log --oneline --graph --all

# Step 3: Create a new branch called "the-beginning" starting from the first commit with message "A" using a detached head
firas@firas-GL65-Leopard-10SCSR:~/Documents/git-katas/ff-merge/exercise$ git switch --detach <commit_hash>
firas@firas-GL65-Leopard-10SCSR:~/Documents/git-katas/ff-merge/exercise$ git branch the-beginning

# Step 4: Restore normalcy by moving to the "master" branch
firas@firas-GL65-Leopard-10SCSR:~/Documents/git-katas/ff-merge/exercise$ git checkout master

# Optional: Check the status and commit history again
firas@firas-GL65-Leopard-10SCSR:~/Documents/git-katas/ff-merge/exercise$ git status
firas@firas-GL65-Leopard-10SCSR:~/Documents/git-katas/ff-merge/exercise$ git log --oneline --graph --all
```

# third exercise : 
```bash
Certainly! Here's the entire sequence of commands in one code block:

# Create a branch called greeting and switch to it
git checkout -b greeting

# Edit the greeting.txt file to contain your favorite greeting
# (Modify greeting.txt with your favorite greeting)

# Add greeting.txt to the staging area and commit
git add greeting.txt
git commit -m "Add greeting.txt"

# Switch back to the master branch
git checkout master

# Create a file README.md with information about this repository
echo "Git Juggling Repository" > README.md
echo "This repository contains examples of lightweight branch juggling in Git." >> README.md

# Add the README.md file to the staging area and commit
git add README.md
git commit -m "committing the readme.md"

# View the Git log
git log --oneline --graph --all

# Diff the branches
git diff master greeting

# Merge the greeting branch into master
git merge greeting

# View the Git log again to see the extra merge commit
git log --oneline --graph --all
```

# fourth exercise : 
```bash
cd merge-mergesort/
source setup.sh

# Create a new branch 'Mergesort-Impl' and implement mergesort
git checkout -b Mergesort-Impl
# (Modify mergesort.py to implement mergesort)
git add mergesort.py
git commit -m "Mergesort implemented on feature branch"

# Switch back to the master branch and make some changes
git checkout master
touch README.md
echo "this repo is going to take some exercises in git" > README.md
git commit -am "committing the readme.md"

# Merge the 'Mergesort-Impl' branch into 'master' (conflict occurs)
git merge Mergesort-Impl
# (Resolve the merge conflict in mergesort.py)
git add mergesort.py
git commit -m "committing"

# View the Git log with 'git lol' and status
git lol
git status
```
