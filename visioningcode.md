# Notes cours visioning code
## Github

## Sur notre machine

On crée un fichier pour faire notre projet

1. créer un compte github
2. create a repository (public except if you have a premium account) with simple name
3. we copy the url which allows us to enter in the depot

## On our pc

We create a folder to do our project

```bash
mkdir <nom_fichier>
cd <nom_fichier>
```

After being in the folder, we turn on the git

`git init`

We check that the git is initialized by doing this command

`ls -a`

We also check that the version of the git, just in case..

`git --version`

### !! Warning !! don't do 
```bash
git remote add https://github.com/Delta-001/visioningcode.git
```
Because "remote add" will send the WHOLE pc to the repositories

### We need to do 
```bash
git remote add origin https://github.com/Delta-001/visioningcode.git
```
So it will only send the origin folder, the source folder

## We will create and push a folder

Even if we did this command, we only told GIT that we're about to connect and now we need to prove that we are autorized to enter in the GIT

`nano file.txt`
to create a file

Principle of GIT / it's like sending a letter by the post office

#### 1. Add files / add a letter to an envelop
    git add
- #### 1.2 Identification
```bash
git config user.email <user@email>
git config user.name <user.name>
```
Il faut faire les deux commandes
#### 2. Address the files / put an address on the envelope 
```bash
git commit -m <explicite message to indicate what is being sended>
```


#### 3. send the files / send the envelope
```bash
git push origin <branchName>
```
Le nom de la branche est visible en faisant `git status`
- #### 3.2 Authentification
```bash
https => identifiant / passwd (token)
ssh => automatic
```

### Création de token
1. Aller sur github puis cliquer sur le profil en haut a droite
2. Aller dans settings
3. Dans le menu à gauche, descendre tout en bas and click on developer settings
4. Develop the personal access tokens and choose the 2nd one
5. create a token by choosing the 2nd options again
6. Check on everything
7. Save the token in a text file (important)

Add/delete/modify