---
id: hsexo3oyat3jze1ub6bf90o
title: Remote Vault
desc: ''
updated: 1677569568901
created: 1676815576383
---
A remote vault is not saved on your local drive but on the internet, e.g. GitHub.

To setup a remote vault you need a GitHub account.

Once you have that you can convert your local vault to remote vault.

An explanation is in the **[Dendron Wiki](https://wiki.dendron.so/notes/6682fca0-65ed-402c-8634-94cd51463cc4/#convert-vault)**

-------
In order to refresh the remote vault you need to have your computer connected to yout GitHub account

To be able to automatically connect to GitHub you need to link your .ssh-key to you GitHub account:

- Go to your ssh-folder (should be in the user folder)
- Copy the text inside of your .pub file
- Go to "Settings" in your GitHub account and add the conent of your .pub-ssh-key
![](/assets/images/2023-02-19-15-55-24.png){max-width: 600px, border: 2px solid gray}

------
If you don't have a ssh-key you need to create one one your pc.

``` sh
ssh-keygen
```

or on mac

``` sh
ssh-keygen -t rsa -b 4096
```
If you didn't have a ssh-key you like need to add GitHub as known host:
```sh
ssh-keyscan github.com >> ~/.ssh/known_hosts
```
----
When updating the remote vault, don't forget to write a message. Otherwise it'll fail.
