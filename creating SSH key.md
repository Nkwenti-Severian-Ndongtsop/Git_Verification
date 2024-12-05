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
 
![Step1](image1.png)

> ### click on the 'settings' option

![step2](next.png)

> ### take the 'SSH and GPG keys' option

![step3](image2.png)

> ### then click on 'New SSH key'

![step4](image3.png)

> ### input a title name, then finally you use `ctrl v` to paste the key you copied using xclip command

![step5](image4.png)

> ### After that you press on Add SSH  key 