## To get started you need to generate an GPG key pair, in case you don't have one.
To generate a GPG key, we use the command\
`gpg --full-generate-key`
 
> ### you will get a prompt with steps to follow as shown below:
 
![guide](new1.png)

#### if you face any difficulty, can check this link for more details [generating GPG keys](https://docs.github.com/en/authentication/managing-commit-signature-verification/generating-a-new-gpg-key)

assuming you have created the key and copied as indicated in the github-documentation, you need to add the key to your github account
> ### click on the image icon at top right as on the image
 
![Step1](image1.png)

> ### click on the 'settings' option

![step2](next.png)

> ### take the 'SSH and GPG keys' option

![step3](image2.png)

> ### then click on 'New GPG key'

![step4](new2.png)

> ### input a title name, then finally you use `ctrl v` to paste the key you copied

![step5](new3.png)

> ### After that you press on Add GPG  key 

### finally you go to you terminal and run this command;

`git config --global commit.gpgsign true`