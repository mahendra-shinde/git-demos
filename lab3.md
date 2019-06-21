## Remote Git Repositories

1. Visit GitHub.com, signup using email address, username, password
    Choose "Free" plan.

2. To Activate your GitHub account, check your INBOX for a welcome mail from GitHub, use the LINK inside email to activate your account.

3. Click "New Repository" and provide repository name, description,
    choose type  "Public"
    Select "ReadMe"
    Add some text in ReadMe file and Click "Commit"

4.  Get the URL for git repository:
    Syntax:
            https://github.com/{ACCOUNT-NAME}/{REPO-NAME}

    example:
            https://github.com/maxunlimited/repo1

5.  Open Command Prompt and download this remote repository:
    $ D:        or  $ cd /d/
    $ cd myrepos
    $ git config --global user.name {ACCOUNT-NAME}
    $ git config --global user.email {EMAIL}
    $ git clone https://github.com/maxunlimited/repo1

6.  Edit the readme file.

    $ cd repo1
    $ notepad README.md

7.  Save changes, commit and push

    $ git add .
    $ git commit -m "Updated Readme!"
    $ git push

    Enter your GITHub password.


