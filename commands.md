# Git Commands Practice Log

## Initialize a Git Repository

### Command
```bash
mkdir git-devops
cd git-devops
git init
```

### Explanation
- Creates a new directory named `git-devops`.
- Moves into the directory.
- Initializes an empty Git repository.

### Expected Output
```bash
Initialized empty Git repository in /home/user/git-devops/.git/
```

---

## Check Repository Status

### Command
```bash
git status
```

### Explanation
Displays the current state of the working directory and staging area.

### Expected Output
```bash
On branch master

No commits yet

nothing to commit
```

---

## Create Multiple Files

### Command
```bash
touch file{1..4}.txt
ls
```

### Explanation
Creates four text files and lists them.

### Expected Output
```bash
file1.txt  file2.txt  file3.txt  file4.txt
```

---

## Add Files to Staging Area

### Command
```bash
git add file1.txt file2.txt
git status
```

### Explanation
Stages file1.txt and file2.txt for commit.

### Expected Output
```bash
Changes to be committed:
  new file: file1.txt
  new file: file2.txt
```

---

## Commit Changes

### Command
```bash
git commit -m "2 file added"
```

### Explanation
Creates a commit containing the staged files.

### Expected Output
```bash
[master (root-commit)] 2 file added
```

---

## View Commit History

### Command
```bash
git log
```

### Explanation
Shows detailed commit history.

---

## Create a New Branch

### Command
```bash
git checkout -b dev
```

### Explanation
Creates and switches to the `dev` branch.

### Expected Output
```bash
Switched to a new branch 'dev'
```

---

## Switch Between Branches

### Command
```bash
git checkout master
git checkout dev
```

### Explanation
Switches between existing branches.

---

## Create and Commit a File in Dev Branch

### Command
```bash
touch file.txt
git add file.txt
git commit -m "added file"
```

### Explanation
Creates a file, stages it, and commits it in the dev branch.

---

## View Commit History in One Line

### Command
```bash
git log --oneline
```

### Explanation
Displays commits in a compact format.

### Expected Output
```bash
abc1234 added file
xyz5678 2 file added
```

---

## List All Branches

### Command
```bash
git branch
```

### Explanation
Shows all local branches.

### Expected Output
```bash
* dev
  master
```

---

## Remove Files

### Command
```bash
rm file3.txt file4.txt
ls
```

### Explanation
Deletes file3.txt and file4.txt and lists remaining files.

### Expected Output
```bash
file1.txt file2.txt file.txt
```

---

## View Command History

### Command
```bash
history
```

### Explanation
Displays previously executed terminal commands.
