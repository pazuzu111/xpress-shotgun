# express-shotgun

# before use
Install bash

Bash version can be queried with the --version flag: 

$ bash --version
3.2.53(1)-release

The actual installation is going to happen with HomeBrew, the OS X package manager, if you don’t have it, installed it with the following command:
$ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

Update homebrew packet database and install bash:
$ brew update && brew install bash

# Add the new shell to the list of allowed shells
sudo bash -c 'echo /usr/local/bin/bash >> /etc/shells'

# Change to the new shell
chsh -s /usr/local/bin/bash 

# Now close terminal and boot the machine!!!!!!

express-shotgun is a npm module that shotguns an express MVC to you rspecified directory
run 
npm install shotgun 

once installed run
express-shotgun nameOfApp nameOfMvcMethods

a directory will be made along with 
the model with methods and sql commands already embedded
the controller & thw views

after you run express-shotgun nameOfApp nameOfMvcMethods
you will hav a full crud express app, all you have to do is create a database, config file, and a node server


# dependecies

```ssh
"ejs": "^2.5.7",
"express": "^4.16.2",
"pg-promise": "^7.0.3"
```

shotgun installs these dependecies for you***
