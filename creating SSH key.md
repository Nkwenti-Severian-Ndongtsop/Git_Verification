# How to verify your commits on github using SSH and GPG keys
## To get started you need to generate an SSH key pair, in case you don't have one.
To generate an ssh key pair we use the following command
`ssh-keygen -t \<type> -b \<bits> -C \<email>

The command is very specific;
> \<type> is the type of key such as (rsa, dsa, ecdsa, ed25519)

> \<bits> is the bit-size which depends on the key type and is applicable only on: rsa, dsa

> \<email> is the email account you want the key to be attached to 

for more detail information on how to create an ssh key, visit the link [how to generate SSH keys](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

After generating the key, you need to add it to the ssh agent using the command\
`eval "$(ssh-agent -s)"`\
activates the agent\

`ssh-add ~/.ssh/<key>`\
adds the key to the agent

you now need to install xclip using\ 
`sudo apt install xclip`

then this command is to copy the key to your clipboard\
`cat ~/.ssh/<public_key> | xclip -selection cipboard`
 
 Finally you need to add the key to your account on github following this steps:\
> ### click on the image icon at top right as on the image
 
![image1](https://github.com/user-attachments/assets/7edb1f1a-aec7-403d-be16-ea21226cb198)

> ### click on the 'settings' option

![next](https://github.com/user-attachments/assets/c945fedb-7a25-4c01-97a7-4832496aec50)

> ### take the 'SSH and GPG keys' option

![image2](https://github.com/user-attachments/assets/c6fc2ab7-4cef-4ee8-9fd4-e58a2a219fc6)

> ### then click on 'New SSH key'

![image3](https://github.com/user-attachments/assets/f40e851b-2588-4a54-813e-d0af510cd292)

> ### input a title name, then finally you use `ctrl v` to paste the key you copied using xclip command

![new3](https://github.com/user-attachments/assets/07720d4d-7fdc-400f-9a84-77c7afb109d9)

> ### After that you press on Add SSH  key 
