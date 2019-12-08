# Setup multiple ssh keys

## On your computer
Create a ssh key setting in a new file and forget to copy the path to the ssh keys directory.

```
ssh-keygen -t rsa -C "super-heroes@mail.com"
Generating public/private rsa key pair.
Enter file in which to save the key (/Users/WonderWoman/.ssh/id_rsa): /Users/WonderWoman/.ssh/id_rsa_heroes
```

Add the new ssh key to ssh service
```
ssh-add ~/.ssh/id_rsa_heroes
```

Check if the key was saved successfully
```
ssh-add -l
```

Copy the public key:
```
pbcopy < ~/.ssh/id_rsa_heroes.pub
```

## On GitHub
Go to Settings > SSH and GPG keys and create a *New SSH key*
Give a meaningful name, paste the public key and press *Add SSH key*

## On your computer

Update ssh configuration file:

```
vi ~/.ssh/config
```

With:
```
#New ssh git account
Host github.com-heroes
	HostName github.com
	User git
	IdentityFile ~/.ssh/id_rsa_heroes
```
Add ssh key:
```
ssh-add -K ~/.ssh/id_rsa_heroes
```

Configured your local account:
```
git config user.name "heroes"
git config user.email "super-heroes@mail.com"
```
