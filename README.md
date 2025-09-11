 create mode 100644 styles.css
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ git status
On branch master
nothing to commit, working tree clean
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ 
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ git branch
* master
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ git branch -m main
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ git branch
* main
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ git branch 
* main
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ ls
image  index.html  styles.css
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ 
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ 
.vishal-gupta@vishal-pc:~/white-stone/test2/tst$ ^C
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ git checkout -b featureproperties/image
Switched to a new branch 'featureproperties/image'
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ git branch
* featureproperties/image
  main
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ ^C
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ ls
image  index.html  styles.css
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ 
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ ls
image  index.html  styles.css
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ mkdir
mkdir: missing operand
Try 'mkdir --help' for more information.
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ 
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ sudo mkdir user-guide
[sudo] password for vishal-gupta: 
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ ls
image  index.html  styles.css  user-guide
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ cd user-guide/
vishal-gupta@vishal-pc:~/white-stone/test2/tst/user-guide$ ls
vishal-gupta@vishal-pc:~/white-stone/test2/tst/user-guide$ touch README.md
touch: cannot touch 'README.md': Permission denied
vishal-gupta@vishal-pc:~/white-stone/test2/tst/user-guide$ sudo touch README.md
vishal-gupta@vishal-pc:~/white-stone/test2/tst/user-guide$ ls
README.md
vishal-gupta@vishal-pc:~/white-stone/test2/tst/user-guide$ code .
vishal-gupta@vishal-pc:~/white-stone/test2/tst/user-guide$ 
vishal-gupta@vishal-pc:~/white-stone/test2/tst/user-guide$ ls
README.md
vishal-gupta@vishal-pc:~/white-stone/test2/tst/user-guide$ cd ..
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ ls
image  index.html  styles.css  user-guide
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ ll
total 76
drwxrwxr-x 6 vishal-gupta vishal-gupta  4096 Sep 12 00:46 ./
drwxrwxr-x 3 vishal-gupta vishal-gupta  4096 Sep 10 04:18 ../
drwxrwxr-x 8 vishal-gupta vishal-gupta  4096 Sep 12 00:21 .git/
drwxrwxr-x 2 vishal-gupta vishal-gupta  4096 Sep 11 22:55 image/
-rw-rw-r-- 1 vishal-gupta vishal-gupta 25870 Sep 11 23:49 index.html
-rw-rw-r-- 1 vishal-gupta vishal-gupta 21180 Sep 11 23:13 styles.css
drwxr-xr-x 2 root         root          4096 Sep 12 00:46 user-guide/
drwxrwxr-x 2 vishal-gupta vishal-gupta  4096 Sep 10 01:29 .vscode/
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ 
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ 
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ git status 
On branch featureproperties/image
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        user-guide/

nothing added to commit but untracked files present (use "git add" to track)
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ git add user-guide/
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ git commit -m "add usier-guide folder for Readme.md"
[featureproperties/image cac92de] add usier-guide folder for Readme.md
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 user-guide/README.md
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ git status
On branch featureproperties/image
nothing to commit, working tree clean
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ git log --onelne
fatal: unrecognized argument: --onelne
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ git log --oneline
cac92de (HEAD -> featureproperties/image) add usier-guide folder for Readme.md
868a44f (main) initial commit
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ 



***************************************************************************************************************************
***************************************************************************************************************************



vishal-gupta@vishal-pc:~/white-stone/test2/tst$ git add .
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   user-guide/README.md

vishal-gupta@vishal-pc:~/white-stone/test2/tst$ git commit -m "v2"
[main c3fcea7] v2
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 user-guide/README.md
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ git branch
  featureproperties/image
* main
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ git checkout featureproperties/image 
Switched to branch 'featureproperties/image'
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ git branch 
* featureproperties/image
  main
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ git checkout main 
Switched to branch 'main'
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ git branch 
  featureproperties/image
* main
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ git status
On branch main
nothing to commit, working tree clean
vishal-gupta@vishal-pc:~/white-stone/test2/tst$ 

+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++



✅ Option 1: Commit the Untracked Files

If you want to keep the changes in main first:

git add user-guide/      # stage the new folder
git commit -m "Add user-guide folder with README.md"


+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

✅ Now you can safely switch to your feature branch:

git checkout featureproperties/image


1️⃣ Check Current Branch & Switch to Main
git branch        # see which branch you're on
git checkout main # switch to main branch
git status        # check if working tree is clean



+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++


2️⃣ Add the New Folder & Commit
git add user-guide/       # stage the new folder and its contents
# OR: git add .            # stage all changes

git commit -m "Add user-guide folder with README.md"
git status                # confirm nothing is left to commit



++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

3️⃣ See Commit History
git log --oneline         # view recent commits


++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++


✅ 1️⃣ Check Git Status

Run:

git status


👉 You should see something like:

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        user-guide/

✅ 2️⃣ Add the New Folder

👉 To add the entire folder and all files inside:

git add user-guide/


👉 Or, simply add everything at once (including any other untracked files):

git add .

✅ 3️⃣ Commit the Changes
git commit -m "Add user-guide folder with README.md"

✅ 4️⃣ Confirm Everything is Committed

👉 Check status again:

git status


Expected output:

✅ 1️⃣ Tell Your Team Member

📋 Example message you can share:

Please do property section development in the branch featureproperties/image.

This section is inside index.html, within the <section id="properties" class="properties"> ... </section> tag.

Make all property-related changes here.

After finishing the work, please commit your changes in this branch using:

git add index.html
git commit -m "Add/update property cards in properties section"


Once done, we will merge the branch into main.

✅ 2️⃣ Team Member Workflow Example

Assuming the team member clones the repo or is already working:

git checkout featureproperties/image
# Edit index.html → work in the properties section
git add index.html
git commit -m "Add new property cards or fix existing ones"

✅ 3️⃣ How You Can Check Changes in This Branch

👉 To see what has changed before merging, run:

git diff main..featureproperties/image


This will show exactly what changed in the index.html compared to main.

✅ 4️⃣ Merge Back After Review

Once everything looks good, as a team lead (or responsible dev), you merge:

git checkout main
git merge featureproperties/image


After that, your main branch will include all the updated properties section code.

✅ Optional: Push to GitHub

If working via GitHub:

1️⃣ Push branch:

git push origin featureproperties/image


2️⃣ Team can create a Pull Request → Code gets reviewed → Merged into main.
