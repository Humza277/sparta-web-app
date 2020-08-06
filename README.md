# What is Jenkins
Continuous integration is a process in which all development work is integrated as early as possible. 
The resulting artifacts are automatically created and tested. This process allows to identify errors in an early stage of the project.

The Jenkins build server is a tool to provide this functionality.
is a popular open source tool to perform continuous integration and build automation. 
Jenkins allows to execute a predefined list of steps, e.g.
    
    su 
    npm install
    node app.js


#How does Jenkins work?
Jenkins works like this:

Developer changes the code: 
    
    The developer commits new code to version control (usually Git or Subversion), and pushes it to the central repo.
Code is delivered to the build server: 
    
    Jenkins monitors the repo continuously. When it sees the new commit, it checks that version of the code out to its server.
Build the application: 
    
    Using build scripts that are also committed to the repo, Jenkins builds the software.
Run the automated tests: 
    
    Unit tests and/or integration tests are also maintained by the development team as part of the same repo. Jenkins uses a test script to run those tests.
Notify developers of problems: 
    
    Jenkins maintains a list of build results that developers can easily view using its web UI. Jenkins can also be set up to e-mail developers when a build fails.
Jenkins can also facilitate continuous delivery or even continuous deployment of your software.

# Accessing private repos
To access a private repo you will need to generate private and public keys this is done by using the keygen command from within your ssh folder
    
    ssh-keygen -t rsa -b 4096
   
# Webhooks 
A webhook API  is a way for an app to provide other applications with real-time information. 
Webhooks delivers data to other applications as it happens, meaning you get data immediately.

Webhooks allow you to build or set up integrations, such as GitHub which subscribe to certain events on GitHub.com. 
When one of those events is triggered, we'll send a HTTP POST payload to the webhook's configured URL.


To add a web hook to your repo 
    
    Open your Repo
    
    Navigate to the settings tab
    
    Click on Webhooks
    
    Add the URL you want
    
    Define the triggers
    
    Then click add
    
You have now made a webhook for your repo

bob 1