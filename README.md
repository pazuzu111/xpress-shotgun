![shotgunlogo1](https://user-images.githubusercontent.com/31411569/34085481-88fdc1ae-e35f-11e7-81d8-bf4fdf9bd516.png)


# xpress-shotgun
xpress-shotgun is an npm module that shotguns an express MVC to your specified directory
  
  * a directory will be made along with the model, with methods and sql commands already embedded
    the controller & the views
  
  * you will have a full crud express app, all you have to do is create a database, a node server, 
    & fll out views to your liking
    
# before use INSTALL bash

Bash version can be queried with the --version flag: 

```sh
bash --version
```
output -> 3.2.53(1)-release

The actual installation is going to happen with HomeBrew, the OS X package manager, if you don’t have it, installed it with the following command:
```sh
1) ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Update homebrew packet database and install bash:
```sh
2) brew update && brew install bash
```

Add the new shell to the list of allowed shells
```sh
3) sudo bash -c 'echo /usr/local/bin/bash >> /etc/shells'
```
Change to the new shell
```sh
chsh -s /usr/local/bin/bash 
```

# Now close terminal and open again
install shotgun GLOBALY:
```sh
npm install -g xpress-shotgun 
```
once installed run:
```sh
shotgun nameofapp dbname modelname(capital) controllername(plural) singularRESPONSE
```
# dependecies

```ssh
"ejs": "^2.5.7",
"express": "^4.16.2",
"pg-promise": "^7.0.3"
```

shotgun installs these dependecies for you***
