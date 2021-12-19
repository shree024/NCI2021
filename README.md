# NCI2021
X20206283 Blockchain Project

This is the readme for this project. It includes all the useful links and commands to run.

# Prerequisites 
-> Visual Studio Code
-> NodeJs
-> Git

Download and Install Visual Studio Code
https://code.visualstudio.com/Download

Create a github account and install Git locally
https://github.com/git-guides/install-git

Install NodeJs
https://nodejs.org/en/download/


# Important Project URLs
GitHub Repo - https://github.com/shree024/NCI2021.git
Docker Repo - https://hub.docker.com/repository/docker/20206283/bclab2021/general


# To run this project using the Github Repo
->  Clone the Repository
    -Verify if Git is installed
        $ git version
    
    -Open VScode, Goto Terminal, Create a folder and go into that folder using the following commands:
        $ mkdir <folder_name>
        $ cd <folder_name>
    
    -Inside that folder, run the command to clone the repo
        $ git clone https://github.com/shree024/NCI2021.git

->  Verify if NPM and all the other dependencies are installed on the system
    -Verify/Install nodeJS
        $ node -v
    
    -Verify/Install npm
        $ npm -v
    
    -Verify/Install Dependencies in package.json file
        $ npm install <package name>

-> Run the following .js files
    -contract.js > to connect to web3 and to Ropsten test network.
        $ node contract.js
    
    -method.js > This calls the transfer method in the erc20 contract for doing the distribution.
        $ node method.js
    
    -distribute.js > To Distribute the token to 10 accounts listed in accounts.txt file at 5% each.
        $ node distribute.js
    
    -handlers.js > To enable a web server, to trigger the distribution by sending a call to localhost:8080/distribute, instead of a manual call to distribute.js inside the docker container.
        $ node handlers.js
    
    -transfer.js > To transfer the token from contract to metamask
        $ node transfer.js


