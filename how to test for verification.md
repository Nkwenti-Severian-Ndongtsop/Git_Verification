After creating and adding the SSH and GPG key to your github account; you amy want to test that it works as expected

Firstly you need to create a new repository, and you clone it using **ssh** and not https

The url will look like this **"git@github.com:<username>/<repository_name>.git"** 

after creating the repository, copy the ssh url and you open your terminal;

use this command to clone the repos to your local machine\
`git clone git@github.com:<username>/<repository_name>.git`
 
 After cloning you do the changes you want to do, using git commands then you commit

 When commiting use the command;

 `git commit -s -m "commit message"`
  
  if you included a passphrase will you be prompted for it except otherwise

  then you push and go on the gui and check 

> ## go to the repository and click on commit link and check if you will see verified

![check](new.4png)

> ## the second commit and first commit on the image are "commit links"
   
> ## When you click on any of them, if your commit was verified you will see verified as on image below

![verified](new5.png)

