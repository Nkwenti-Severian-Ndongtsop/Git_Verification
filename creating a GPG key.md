## To get started you need to generate an GPG key pair, in case you don't have one.
To generate a GPG key, we use the command\
`gpg --full-generate-key`
 
> ### you will get a prompt with steps to follow as shown below:
 
![guide](new1.png)

#### if you face any difficulty, can check this link for more details [generating GPG keys](https://docs.github.com/en/authentication/managing-commit-signature-verification/generating-a-new-gpg-key)

assuming you have created the key and copied as indicated in the github-documentation, you need to add the key to your github account
> ### click on the image icon at top right as on the image
 
![image1](https://github.com/user-attachments/assets/15111644-9c12-44be-a4ac-c1cb7572112e)

> ### click on the 'settings' option

![next](https://github.com/user-attachments/assets/8f88e658-33a3-49f2-9f45-89967d6299db)

> ### take the 'SSH and GPG keys' option

![image2](https://github.com/user-attachments/assets/68f4818f-2b8b-4b3c-8498-efad5ffb6e62)

> ### then click on 'New GPG key'

![new2](https://github.com/user-attachments/assets/b35fc6b7-41fa-474b-8d3a-6347c3658f86)

> ### input a title name, then finally you use `ctrl v` to paste the key you copied

![new3](https://github.com/user-attachments/assets/9bfa1aa1-7004-48bc-87b2-9a48471f1b17)

> ### After that you press on Add GPG  key 

### finally you go to you terminal and run this command;

`git config --global commit.gpgsign true`
