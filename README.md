![shotgunlogo1](https://user-images.githubusercontent.com/31411569/34085495-c7f82124-e35f-11e7-97de-f0a36cd80ad2.png)
![ezgif com-video-to-gif 1](https://user-images.githubusercontent.com/31411569/34190621-cb417db0-e50f-11e7-8077-d0b36d3e706c.gif)

# xpress-shotgun
xpress-shotgun is a npm module that shotguns an express MVC to your specified directory
  
  * a directory will be made along with the model, with methods and sql commands already embedded
    the controller & the views
  
  * you will have a full crud express app, all you have to do is create a database, a node server, 
    & fll out views to your liking
    
  * shotgun also takes care of the npm init & installs ejs(viewengine) and pg-promise(more info below)

    
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

# installation

install shotgun GLOBALLY:
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

# PG promise 

PG-PROMISE grants you accesss to DB query methods
  * Automatic connections
  * Automatic transactions
  * Powerful query-formatting engine
  * Support for ES6 generators and ES7 async/await
  * Declarative approach to handling query results
  * Global events reporting for central handling
  * Extensive support for external SQL files
  * Support for all promise libraries

# examples
* Simple SELECT

# ES5
```ssh
db.any('SELECT * FROM users WHERE active = $1', [true])
    .then(function(data) {
        // success;
    })
    .catch(function(error) {
        // error;
    });
  ```
# ES6
```ssh
try {
    const users = yield db.any('SELECT * FROM users WHERE active = $1', [true]);
    // success
} 
catch(e) {
   // error
}
```
# ES7
```ssh
try {
    const users = await db.any('SELECT * FROM users WHERE active = $1', [true]);
    // success
} 
catch(e) {
    // error
}
```

****************************************************************************************
# ejs

Features

  * Control flow with <% %>
  * Escaped output with <%= %> (escape function configurable)
  * Unescaped raw output with <%- %>
  * Newline-trim mode ('newline slurping') with -%> ending tag
  * Whitespace-trim mode (slurp all whitespace) for control flow with <%_ _%>
  * Custom delimiters (e.g., use <? ?> instead of <% %>)
  * Includes
  * Client-side support
  * Static caching of intermediate JavaScript
  * Static caching of templates
  * Complies with the Express view system
  
# Examples
```ssh
<% if (user) { %>
  <h2><%= user.name %></h2>
<% } %>
Try EJS online at: https://ionicabizau.github.io/ejs-playground/.
```
# Usage
```ssh
var template = ejs.compile(str, options);
template(data);
// => Rendered HTML string 
 
ejs.render(str, data, options);
// => Rendered HTML string 
 
ejs.renderFile(filename, data, options, function(err, str){
    // str => Rendered HTML string 
});
```
