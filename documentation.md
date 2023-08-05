
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
