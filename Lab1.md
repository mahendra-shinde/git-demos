## LAB 1:  Setting up GIT and Creating Repository

Objective : Install GIT and create simple repository

Pre-requisites: Windows OS with Internet Connection
                Admin privileges for installation

1. Verify GIT Installation

    Open Command Prompt, and try command "GIT"

2. Download Git for Windows from https://git-scm.com/download/win
3. Run the Installer to install GIT

4. Configure GIT environment using command: (One Time Task)
    $ git config --global user.name "Mahendra Shinde"
    $ git config --global user.email "MahendraShinde@synergetics-india.com"

5. Create a new Repository
    $ D:   
    $ mkdir \myrepos
    $ cd \myrepos
    $ git init myproject1
    $ cd myproject1
    $ notepad page1.html

6.  Notepad would complain that file "page1.html" DO NOT exists!
    Do you want to create new ? Press Yes or OK
    Add following text:
        <h2>Hello World</h2>

7.  Save and Close Notepad and return back to command Prompt
    $ git status
    $ git add page1.html
    $ git commit -m "First Change!"