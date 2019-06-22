### Lab 2 : Settin up Maven Based Java Application

1.  Access Jenkins Dashboard from Web Browser
2.  Login Using newly created user account (Refer Lab 1)
3.  Manage Jenkins > Global Tool Configuration
        
        Locate "Maven"
        Click "Add Maven" > "Maven Installations"
            Name: maven3
            Version: 3.6.0 from Apache
        Click Save 

3.  Back to Dashboard, Click New Item > 

        Name: java-app1
        Type: Freestyle project
    
4.  Source Code Management TAB:
        
        Choose "Git"
        Enter Repository path:
        
            https://github.com/mahendra-shinde/ci-demo

5.  Choose Build TAB
        
        Choose Maven version "maven3"
        Goal : clean package
        Click on "Advanced" button
        and Write POM location : DemoApp/pom.xml

        Click Save
