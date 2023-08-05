
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

Please replace `<commit_hash>` with the actual commit hash of the first commit with the message "A." Remember to follow the commands in order, and the "the-beginning" branch should be created starting from the desired commit.
