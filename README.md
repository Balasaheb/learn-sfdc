# OneTime Setup (Git Repository and SFDX Project Setup)

## Cloning Repository 
Cloning repository means setting up your local environment and pull code from remote repository (FROM GITHUB.COM ), This is one time setup and you need to perform only once per repository, Follow below steps 

1) Open VS Code new window and open terminal window, using cd command , navigate to desired folder

    `cd SalesforceBasics`

    now you are inside [SalesforceBasics] folder
    
2) Now clone our repository from remote server with below command  , it will clone repository to local
    `git clone https://github.com/Balasaheb/learn-sfdc.git`
3) Navigate to folder structure using `cd learn-sfdc` 
4) Use `git branch` and make sure you have GIT initialized there.
5) Now checkout master branch with below commands (One by One), It will fetch code from master branch to local folder 
    `git checkout master`
    `git fetch --all`
    
Now your local files are loaded with remote codebase


## Create Salesforce DX Project

### Assuming You are already authorized to your DEV-HUB account !

Now you have codebase from remote repository , we need to create SFDX project and push it to scratch Org
1) You are still in "NEW VS Code Window mode" , use [Open Folder] button from right side explorer window and [learn-sfdc] folder in your VS code
2) Again use `git branch` , `git fetch --all` , `git pull --all` commands to keep your local files upto date
 [Congratulations] your SFDX project is ready to use

## Create Scratch Org and Push source code to it
1) Use [Ctrl+Shift+P] to open pallete window and Use `SFDX : Create Default Scratch Org` command to create new scratch Org
2) Use `SFDX : Push Source To Default Scratch Org and Override Conflicts` , It will deploy code to scratch Org 
3) Use `sfdx force:org:open` to open your scratch ORG and start using it 


#### Congratulations , you have successfully cloned remote repository and created scratch Org using same source code 


# Day To Day working with GIT 

## Checkout master branch 
`git checkout master`

`git pull origin master`


Now your local files are upto date with master , deploy it to desired or new scratch org as per need

Create new feature branch 

`git checkout -b feature/MyModuleone`


Add files 

`git add *`    // adding all changed files 


`git add FILE_PATH`  // adding individual files 

`git commit -m "Adding some message " `  // Adding message to commit 

`git push origin feature/MyModuleOne`  // Pushing changes to repo 

Now create Pull request and get merged with master branch 





## Read All About It

- [Salesforce Extensions Documentation](https://developer.salesforce.com/tools/vscode/)
- [Salesforce CLI Setup Guide](https://developer.salesforce.com/docs/atlas.en-us.sfdx_setup.meta/sfdx_setup/sfdx_setup_intro.htm)
- [Salesforce DX Developer Guide](https://developer.salesforce.com/docs/atlas.en-us.sfdx_dev.meta/sfdx_dev/sfdx_dev_intro.htm)
- [Salesforce CLI Command Reference](https://developer.salesforce.com/docs/atlas.en-us.sfdx_cli_reference.meta/sfdx_cli_reference/cli_reference.htm)
