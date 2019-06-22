Lab 1 : Setting up Jenkins Environment

1. Import the OVA file into Virtual Box (10 Minutes)

2. Start The VM 

3. Wait for the screen to display Jenkins Username, password and IP address

4. Open Web Browser and Visit the IP address 

    ex. http://192.168.8.101/

5.  After wait for may be 3/4 minutes you should get jenkins dashboard giving 
    TWO options for plugins installation:
    
        1. Install Recommanded/Suggested Plugins
        2. Install Selected pluginning (Choose This)
            Choose "NONE" for plugins
            Choose "GIT" then Install

6.  User name & Password for Login:
    
    Get username and password for VirtualBox VM
    HINT: Username is "user"

7.  Goto "Manage Jenkins" > "Manage Users" > Create User
    Enter user details

8.  Go back to Jenkins Dashboard and click on "New Item"
    
    Type: Freestyle project
    Name: project1

9.  Under General TAB:
    
    Write Description for current project 

10. Source Code Management TAB:
    
    Choose NONE

11. Build Triggers TAB:
    
    Choose "Build Periodically"
    Pattern: * * * * *

12. Build TAB:
    
    Choose from Drop Down: "Execute Shell" 
    
    NOTE: On Windows System use "Execute Windows Batch Command"

    Write the Shell script:
    
        ```
        echo "Building $JOB_NAME"
        echo "Hello World"
        ```
13. Click SAVE button.
