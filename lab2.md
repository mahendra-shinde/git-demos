
Switch to D Drive (CMD prompt)
$ D:

Switch to D Drive (Bash/MingW prompt)
$ cd /d/

Open file for editing
$ cd myrepos/myproject1
$ notepad page1.html
OR
$ vi page1.html

Replace "world" with "India"
And Save & Close the file (Notepad or VI)

Capture changes and add to staging area (. = All files & directories)
$ git add .

Do a new commit
$ git commit -m "Second change!"

List of Commits
$ git log

Compare TWO commits
$ git diff {COMMIT1} {COMMIT2}

Replace {COMMIT1} with FIRST FOUR characters of Commit ID #1
Replace {COMMIT2} with FIRST FOUR characters of Commit ID #2

Made a new Branch "dev"
$ git branch dev

List all branches ?
$ git branch

Switch to new branch
$ git checkout dev

Open page1.html and make few changes
Use git add and git commit
$ git add .
$ git commit -m "Third commit"

Switch back to MASTER branch
$ git checkout master

Open page1.html
$ notepad page1.html

Switch to dev branch and check file contents
$ git checkout dev
$ notepad page1.html