# **Git Commands**

## **Setup**

### **Configuring user information used across all local repositories.**

-   **$ git config --global user.name "[firstname lastname]" - Set a name that is identifable for credit when review version history.**
-   **$ git config --global user.email "[valid-email]" - Set an email address that will be associated with each history maker.**
-   **$ git config --global color.ui auto - Set automatic command line coloring for Git for easy reviewing.**

---

## **Setup & Init**

### **Configuring user information, initializing and cloning repositories.**

-   **$ git init - Initialize an existing directory as a Git repository.**
-   **$ git clone [url] - Retrieve an entire repository from a hosted location via URL.**

---

## **Stage & Snapshot**

### **Working with snapshots and the Git staging area.**

-   **$ git status - Show modified files in working directory, staged for your next commit.**
-   **$ git add [file] - Add a file as it looks now to your next commit (stage).**
-   **$ git reset [file] - Unstage a file while retaining the changes in working directory.**
-   **$ git diff - diff of what is changed but not staged.**
-   **$ git diff --staged - Diff of what is staged but not yet commited.**
-   **$ git commit -m "[descriptive message]" - Commit your staged content as a new commit snapshot.**

---

## **Branch & Merge**

### **Isolating work in branches, changing context, and integrating changes.**

-   **$ git branch - List your branches.a will appear next to the currently active branch.**
-   **$ git branch [branch-name] - Create a new branch at the current commit.**
-   **$ git checkout - Switch to another branch and check it out into your working directory.**
-   **$ git merge [branch] - Merge the specified branch's history into the current one.**
-   **$ git log - Show all commits in the current branch's history.**

---

## **Incpect & Compare**

### **Examining logs, diffs and object information.**

-   **$ git log - Show the commit history for the currently active branch.**
-   **$ git log branchB..branchA - Show the commits on branchA that are not on branchB.**
-   **$ git log --follow [file] - Show the commits that changed file, even across renames.**
-   **$ git diff branchB..branchA - Show the diss of what is a branchB that is not in branchB.**
-   **$ git show [SHA] - Show any object in Git in human-readable format.**

---

## **Tracking Path Changes**

### **Versioning file removes and path changes.**

-   **$ git rm [file] - Delete the file from project and stage the removal from commit.**
-   **$ git mv [existing-path] [new-path] - Change an exisiting file path and stage the move.**
-   **$ git log --start -M - Show all commit logs with indication of any paths that moved.**

---

## **Ignoring Patterns**

### **Preventins inintentional staging or commiting of files.**

-   **$ git config --global core.excludesfile [file] - System wide ignore pattern for all local repositories.**

---

## **Share & Update**

### **Retrieving updated from another repository and updating local repos.**

-   **$ git remote add [alias] [url] - Add a git URL as an alias.**
-   **$ git fetch [alias] - Fetch down all the branches from that Git remote.**
-   **$ git merge [alias]/[branch] - Merge a remote branch into your current branch to bring it up to date.**
-   **$ git push [alias] [branch] - Transmit local branch commits to the remote repository branch.**
-   **$ git pull - Fetch and merge any commits from the tracking remote branch.**

---

## **Rewrite History**

### **Rewriting branches, updating commits and clearing history.**

-   **$ git rebase [branch] - Apply any commits of current branch ahead of specified one.**
-   **$ git reset --hard [commit] - Clear staging area, rewrite working tree from specified commit.**

---

## **Temporary Commits**

### **Temporary store modified, tracked files in order to change branches.**

-   **$ git stash - Save modified and staged changes.**
-   **$ git stash list - List stack-order of stashed file changes.**
-   **$ git stash pop - Write working from top of stash stack.**
-   **$ git stash drop - Discard the changes from top of stash stack.**
