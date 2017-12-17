# express-shotgun

# before use
Install bash

Bash version can be queried with the --version flag: 

```sh
bash --version
```
output -> 3.2.53(1)-release

The actual installation is going to happen with HomeBrew, the OS X package manager, if you don’t have it, installed it with the following command:
```sh
$ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Update homebrew packet database and install bash:
```sh
brew update && brew install bash
```

Add the new shell to the list of allowed shells
```sh
sudo bash -c 'echo /usr/local/bin/bash >> /etc/shells'
```
Change to the new shell
```sh
chsh -s /usr/local/bin/bash 
```

# Now close terminal and open again

express-shotgun is a npm module that shotguns an express MVC to your specified directory
install GLOBALY:
```sh
npm install -g xpress-shotgun 
```
once installed run:
```sh
shotgun nameofapp dbname modelname(capital) controllername(plural) singularRESPONSE
```
- a directory will be made along with the model, with methods and sql commands already embedded
  the controller & the views

- you will have a full crud express app, all you have to do is create a database, a node server, 
  & fll out views to your liking

# dependecies

```ssh
"ejs": "^2.5.7",
"express": "^4.16.2",
"pg-promise": "^7.0.3"
```

shotgun installs these dependecies for you***
