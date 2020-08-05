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