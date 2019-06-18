# sample-web-server
テクノロジー（藤原）Node.jsによるサンプルWebサーバ

```
yamadamasakinoMacBook-Pro:~ boshy$ cat ~/.bash_profile

# Setting PATH for Python 3.7
# The original version is saved in .bash_profile.pysave
PATH="/Library/Frameworks/Python.framework/Versions/3.7/bin:${PATH}"
export PATH
export PATH=$PATH:/Applications/MAMP/Library/bin

You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:~ boshy$ cd ~/fujiwara
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:fujiwara boshy$ git clone git@github.com:yamadayuuya/sample-web-server.git
Cloning into 'sample-web-server'...
remote: Enumerating objects: 7, done.
remote: Counting objects: 100% (7/7), done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 7 (delta 1), reused 5 (delta 1), pack-reused 0
Receiving objects: 100% (7/7), done.
Resolving deltas: 100% (1/1), done.
yamadamasakinoMacBook-Pro:fujiwara boshy$ code .
yamadamasakinoMacBook-Pro:fujiwara boshy$ curl --silent --requwst GET --url https://api.thecatapi.com/v1/images/search
curl: option --requwst: is unknown
curl: try 'curl --help' or 'curl --manual' for more information
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:fujiwara boshy$ curl --silent --request GET --url https://api.thecatapi.com/v1/images/search
[{"breeds":[],"categories":[{"id":15,"name":"clothes"}],"id":"MTgwMTIzMA","url":"https://cdn2.thecatapi.com/images/MTgwMTIzMA.jpg","width":800,"height":531}]You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:fujiwara boshy$ curl --silent --request GET --url 'https://api.thecatapi.com/v1/images/search?limit=3'
[{"breeds":[],"id":"bbf","url":"https://cdn2.thecatapi.com/images/bbf.jpg","width":400,"height":265},{"breeds":[],"id":"btk","url":"https://cdn2.thecatapi.com/images/btk.jpg","width":650,"height":494},{"breeds":[],"id":"MTkyNjU3NQ","url":"https://cdn2.thecatapi.com/images/MTkyNjU3NQ.jpg","width":500,"height":375}]You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:fujiwara boshy$ curl --silent --request GET --url 'https://api.thecatapi.com/v1/images/search?limit=5'
[{"breeds":[],"id":"75k","url":"https://cdn2.thecatapi.com/images/75k.jpg","width":500,"height":381},{"breeds":[],"id":"MTY2NDU1Mw","url":"https://cdn2.thecatapi.com/images/MTY2NDU1Mw.jpg","width":1920,"height":1280},{"breeds":[],"id":"MTk5NTUzNA","url":"https://cdn2.thecatapi.com/images/MTk5NTUzNA.jpg","width":760,"height":884},{"breeds":[],"id":"XghEh4zcU","url":"https://cdn2.thecatapi.com/images/XghEh4zcU.jpg","width":564,"height":988},{"breeds":[],"id":"fWfGwt24O","url":"https://cdn2.thecatapi.com/images/fWfGwt24O.jpg","width":1280,"height":852}]yamadamasakinoMacBook-Pro:fujiwara boshy$ brew install jq
Updating Homebrew...
^CError: The following directories are not writable by your user:
/usr/local/lib/pkgconfig

You should change the ownership of these directories to your user.
  sudo chown -R $(whoami) /usr/local/lib/pkgconfig

And make sure that your user has write permission.
  chmod u+w /usr/local/lib/pkgconfig
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:fujiwara boshy$ brew install jq
Updating Homebrew...
==> Auto-updated Homebrew!
Updated 1 tap (homebrew/core).
==> New Formulae
swig@3
==> Updated Formulae
aws-sdk-cpp         glib                mighttpd2           scons
braid               glooctl             minio               scrcpy
calicoctl           gmic                minio-mc            ship
certbot             graph-tool          nomad               sops
chakra              gst-plugins-good    opa                 telegraf
circleci            hlint               paket               terraform
envconsul           imagemagick         phpunit             topgrade
exiftool            jdupes              procs               vultr
firebase-cli        jfrog-cli-go        pulumi              webpack
flow                joplin              pybind11            whois
fluxctl             knot                pyenv               wildfly-as
folly               libev               rbspy               wtf
gibo                lmod                scalariform         yelp-tools
==> Deleted Formulae
swig@3.04

Error: The following directories are not writable by your user:
/usr/local/lib/pkgconfig

You should change the ownership of these directories to your user.
  sudo chown -R $(whoami) /usr/local/lib/pkgconfig

And make sure that your user has write permission.
  chmod u+w /usr/local/lib/pkgconfig
yamadamasakinoMacBook-Pro:fujiwara boshy$ brew install jq
Error: The following directories are not writable by your user:
/usr/local/lib/pkgconfig

You should change the ownership of these directories to your user.
  sudo chown -R $(whoami) /usr/local/lib/pkgconfig

And make sure that your user has write permission.
  chmod u+w /usr/local/lib/pkgconfig
yamadamasakinoMacBook-Pro:fujiwara boshy$ brew install jq
Error: The following directories are not writable by your user:
/usr/local/lib/pkgconfig

You should change the ownership of these directories to your user.
  sudo chown -R $(whoami) /usr/local/lib/pkgconfig

And make sure that your user has write permission.
  chmod u+w /usr/local/lib/pkgconfig
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:fujiwara boshy$ brew install jq
Error: The following directories are not writable by your user:
/usr/local/lib/pkgconfig

You should change the ownership of these directories to your user.
  sudo chown -R $(whoami) /usr/local/lib/pkgconfig

And make sure that your user has write permission.
  chmod u+w /usr/local/lib/pkgconfig
yamadamasakinoMacBook-Pro:fujiwara boshy$ curl --silent --request GET --url 'https://api.thecatapi.com/v1/images/search?limit=3' | jq
-bash: jq: command not found
(23) Failed writing body
yamadamasakinoMacBook-Pro:fujiwara boshy$ cd sample-web-server/
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:sample-web-server boshy$ code .
yamadamasakinoMacBook-Pro:sample-web-server boshy$ brew install jq
Error: The following directories are not writable by your user:
/usr/local/lib/pkgconfig

You should change the ownership of these directories to your user.
  sudo chown -R $(whoami) /usr/local/lib/pkgconfig

And make sure that your user has write permission.
  chmod u+w /usr/local/lib/pkgconfig
yamadamasakinoMacBook-Pro:sample-web-server boshy$ brew install jq
Error: The following directories are not writable by your user:
/usr/local/lib/pkgconfig

You should change the ownership of these directories to your user.
  sudo chown -R $(whoami) /usr/local/lib/pkgconfig

And make sure that your user has write permission.
  chmod u+w /usr/local/lib/pkgconfig
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:sample-web-server boshy$ brew install jq
Error: The following directories are not writable by your user:
/usr/local/lib/pkgconfig

You should change the ownership of these directories to your user.
  sudo chown -R $(whoami) /usr/local/lib/pkgconfig

And make sure that your user has write permission.
  chmod u+w /usr/local/lib/pkgconfig
yamadamasakinoMacBook-Pro:sample-web-server boshy$ curl --silent --request GET --url 'https://api.thecatapi.com/v1/images/search?limit=3'
[{"breeds":[],"id":"9ot","url":"https://cdn2.thecatapi.com/images/9ot.jpg","width":612,"height":612},{"breeds":[],"id":"dro","url":"https://cdn2.thecatapi.com/images/dro.jpg","width":604,"height":403},{"breeds":[],"id":"MjAzMTA4Nw","url":"https://cdn2.thecatapi.com/images/MjAzMTA4Nw.jpg","width":720,"height":540}]You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:sample-web-server boshy$ brew install jq
Error: The following directories are not writable by your user:
/usr/local/lib/pkgconfig

You should change the ownership of these directories to your user.
  sudo chown -R $(whoami) /usr/local/lib/pkgconfig

And make sure that your user has write permission.
  chmod u+w /usr/local/lib/pkgconfig
yamadamasakinoMacBook-Pro:sample-web-server boshy$ sudo chown -R $(whoami) /usr/local/lib/pkgconfig
Password:
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:sample-web-server boshy$ brew install jq
==> Installing dependencies for jq: oniguruma
==> Installing jq dependency: oniguruma
==> Downloading https://homebrew.bintray.com/bottles/oniguruma-6.9.2.mojave.bott
==> Downloading from https://akamai.bintray.com/c6/c613befafe81da48913ebd1a7eb03
######################################################################## 100.0%
==> Pouring oniguruma-6.9.2.mojave.bottle.tar.gz
🍺  /usr/local/Cellar/oniguruma/6.9.2: 17 files, 1.3MB
==> Installing jq
==> Downloading https://homebrew.bintray.com/bottles/jq-1.6.mojave.bottle.1.tar.
==> Downloading from https://akamai.bintray.com/71/71f0e76c5b22e5088426c971d5e79
######################################################################## 100.0%
==> Pouring jq-1.6.mojave.bottle.1.tar.gz
🍺  /usr/local/Cellar/jq/1.6: 18 files, 1MB
==> `brew cleanup` has not been run in 30 days, running now...
yamadamasakinoMacBook-Pro:sample-web-server boshy$ curl --silent --request GET --url 'https://api.thecatapi.com/v1/images/search?limit=3' | jq
[
  {
    "breeds": [],
    "id": "bvf",
    "url": "https://cdn2.thecatapi.com/images/bvf.jpg",
    "width": 640,
    "height": 480
  },
  {
    "breeds": [],
    "id": "MjA1MTc4Mw",
    "url": "https://cdn2.thecatapi.com/images/MjA1MTc4Mw.jpg",
    "width": 500,
    "height": 375
  },
  {
    "breeds": [],
    "id": "3-inb9sI1",
    "url": "https://cdn2.thecatapi.com/images/3-inb9sI1.jpg",
    "width": 736,
    "height": 736
  }
]
yamadamasakinoMacBook-Pro:sample-web-server boshy$ curl --silent --request GET --url 'https://api.thecatapi.com/v1/images/search?limit=3' > thecat.json
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:sample-web-server boshy$ curl --silent --request GET --url 'https://api.thecatapi.com/v1/images/search?limit=3' >> thecat.json
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:sample-web-server boshy$ curl --silent --request GET --url 'https://api.thecatapi.com/v1/images/search?limit=3' > thecat.json
yamadamasakinoMacBook-Pro:sample-web-server boshy$ curl --silent --request GET --url 'https://api.thecatapi.com/v1/images/search?limit=3' > thecat.json
yamadamasakinoMacBook-Pro:sample-web-server boshy$ cat ~/.bash_profile

# Setting PATH for Python 3.7
# The original version is saved in .bash_profile.pysave
PATH="/Library/Frameworks/Python.framework/Versions/3.7/bin:${PATH}"
export PATH
export PATH=$PATH:/Applications/MAMP/Library/bin

You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:sample-web-server boshy$ sudo vi .bash_profile
Password:
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:sample-web-server boshy$ sudo vi ~/.bash_profile
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:sample-web-server boshy$ vi ~/.bash_profile
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:sample-web-server boshy$ curl -L git.io/nodebrew | perl - setup
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
  0     0    0     0    0     0      0      0 --:--:--  0:00:01 --:--:--     0
  0     0    0     0    0     0      0      0 --:--:--  0:00:01 --:--:--     0
100 24634  100 24634    0     0  14753      0  0:00:01  0:00:01 --:--:-- 14753
Fetching nodebrew...
Installed nodebrew in $HOME/.nodebrew

========================================
Export a path to nodebrew:

export PATH=$HOME/.nodebrew/current/bin:$PATH
========================================
yamadamasakinoMacBook-Pro:sample-web-server boshy$ export PATH=$HOME/.nodebrew/current/bin:$PATH >> ~/.bashrc
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:sample-web-server boshy$ source ~/.bashrc
yamadamasakinoMacBook-Pro:sample-web-server boshy$ nodebrew
nodebrew 1.0.1

Usage:
    nodebrew help                         Show this message
    nodebrew install <version>            Download and install <version> (from binary)
    nodebrew compile <version>            Download and install <version> (from source)
    nodebrew install-binary <version>     Alias of `install` (For backward compatibility)
    nodebrew uninstall <version>          Uninstall <version>
    nodebrew use <version>                Use <version>
    nodebrew list                         List installed versions
    nodebrew ls                           Alias for `list`
    nodebrew ls-remote                    List remote versions
    nodebrew ls-all                       List remote and installed versions
    nodebrew alias <key> <value>          Set alias
    nodebrew unalias <key>                Remove alias
    nodebrew clean <version> | all        Remove source file
    nodebrew selfupdate                   Update nodebrew
    nodebrew migrate-package <version>    Install global NPM packages contained in <version> to current version
    nodebrew exec <version> -- <command>  Execute <command> using specified <version>

Example:
    # install
    nodebrew install v8.9.4

    # use a specific version number
    nodebrew use v8.9.4
yamadamasakinoMacBook-Pro:sample-web-server boshy$ nodebrew install-binary latest
Fetching: https://nodejs.org/dist/v12.4.0/node-v12.4.0-darwin-x64.tar.gz
######################################################################## 100.0%
Installed successfully
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:sample-web-server boshy$ nodebrew ls
v12.4.0

current: none
yamadamasakinoMacBook-Pro:sample-web-server boshy$ mkdir mywebapi
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:sample-web-server boshy$ cd mywebapi/
yamadamasakinoMacBook-Pro:mywebapi boshy$ npm init
-bash: npm: command not found
yamadamasakinoMacBook-Pro:mywebapi boshy$ npm init
-bash: npm: command not found
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:mywebapi boshy$ npm -v
-bash: npm: command not found
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:mywebapi boshy$ node -v
-bash: node: command not found
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:mywebapi boshy$ cd ..
yamadamasakinoMacBook-Pro:sample-web-server boshy$ nodebrew install-binary latest
v12.4.0 is already installed
yamadamasakinoMacBook-Pro:sample-web-server boshy$ nodebrew ls
v12.4.0

current: none
yamadamasakinoMacBook-Pro:sample-web-server boshy$ nodebrew use latest use v12.4.0
use v12.4.0
yamadamasakinoMacBook-Pro:sample-web-server boshy$ node -v
v12.4.0
yamadamasakinoMacBook-Pro:sample-web-server boshy$ cd mywebapi/
yamadamasakinoMacBook-Pro:mywebapi boshy$ npm init
This utility will walk you through creating a package.json file.
It only covers the most common items, and tries to guess sensible defaults.

See `npm help json` for definitive documentation on these fields
and exactly what they do.

Use `npm install <pkg>` afterwards to install a package and
save it as a dependency in the package.json file.

Press ^C at any time to quit.
package name: (mywebapi) 
version: (1.0.0) 
description: 
entry point: (index.js) 
test command: 
git repository: 
keywords: 
author: 
license: (ISC) 
About to write to /Users/boshy/Documents/fujiwara/sample-web-server/mywebapi/package.json:

{
  "name": "mywebapi",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "author": "",
  "license": "ISC"
}


Is this OK? (yes) 
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:mywebapi boshy$ 
```
You have new mail.
yamadamasakinoMacBook-Pro:~ boshy$ cd fujiwara
yamadamasakinoMacBook-Pro:fujiwara boshy$ ls
hello-git		sample-web-server
learning-http-message	simple-web-site
yamadamasakinoMacBook-Pro:fujiwara boshy$ cd mywebapi
-bash: cd: mywebapi: No such file or directory
yamadamasakinoMacBook-Pro:fujiwara boshy$ sam
-bash: sam: command not found
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:fujiwara boshy$ cd sample-web-server/
yamadamasakinoMacBook-Pro:sample-web-server boshy$ cd mywebapi/
yamadamasakinoMacBook-Pro:mywebapi boshy$ npm install --save express
-bash: npm: command not found
yamadamasakinoMacBook-Pro:mywebapi boshy$ npm init
-bash: npm: command not found
yamadamasakinoMacBook-Pro:mywebapi boshy$ cat ~/.bash_profile

# Setting PATH for Python 3.7
# The original version is saved in .bash_profile.pysave
PATH="/Library/Frameworks/Python.framework/Versions/3.7/bin:${PATH}"
export PATH
export PATH=$PATH:/Applications/MAMP/Library/bin
if [ -f ~/.bashrc ] ; then
  source .bashrc
fi
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:mywebapi boshy$ nodebrew
-bash: nodebrew: command not found
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:mywebapi boshy$ source ~/.bashrc
yamadamasakinoMacBook-Pro:mywebapi boshy$ nodebrew
-bash: nodebrew: command not found
yamadamasakinoMacBook-Pro:mywebapi boshy$ echo "export PATH=$HOME/.nodebrew/current/bin:$PATH" >> ~/.bashrc
yamadamasakinoMacBook-Pro:mywebapi boshy$ nodebrew
-bash: nodebrew: command not found
yamadamasakinoMacBook-Pro:mywebapi boshy$ curl -L git.io/nodebrew | perl - setup
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
  0     0    0     0    0     0      0      0 --:--:--  0:00:01 --:--:--     0
  0     0    0     0    0     0      0      0 --:--:--  0:00:02 --:--:--     0
100 24634  100 24634    0     0   7666      0  0:00:03  0:00:03 --:--:--  7666
Fetching nodebrew...
Installed nodebrew in $HOME/.nodebrew

========================================
Export a path to nodebrew:

export PATH=$HOME/.nodebrew/current/bin:$PATH
========================================
yamadamasakinoMacBook-Pro:mywebapi boshy$ nodebrew
-bash: nodebrew: command not found
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:mywebapi boshy$ source ~/.bashrc
yamadamasakinoMacBook-Pro:mywebapi boshy$ nodebrew
nodebrew 1.0.1

Usage:
    nodebrew help                         Show this message
    nodebrew install <version>            Download and install <version> (from binary)
    nodebrew compile <version>            Download and install <version> (from source)
    nodebrew install-binary <version>     Alias of `install` (For backward compatibility)
    nodebrew uninstall <version>          Uninstall <version>
    nodebrew use <version>                Use <version>
    nodebrew list                         List installed versions
    nodebrew ls                           Alias for `list`
    nodebrew ls-remote                    List remote versions
    nodebrew ls-all                       List remote and installed versions
    nodebrew alias <key> <value>          Set alias
    nodebrew unalias <key>                Remove alias
    nodebrew clean <version> | all        Remove source file
    nodebrew selfupdate                   Update nodebrew
    nodebrew migrate-package <version>    Install global NPM packages contained in <version> to current version
    nodebrew exec <version> -- <command>  Execute <command> using specified <version>

Example:
    # install
    nodebrew install v8.9.4

    # use a specific version number
    nodebrew use v8.9.4
yamadamasakinoMacBook-Pro:mywebapi boshy$ nodebrew ls
v12.4.0

current: v12.4.0
yamadamasakinoMacBook-Pro:mywebapi boshy$ echo "export PATH=$HOME/.nodebrew/current/bin:$PATH" >> ~/.bashrc
You have new mail in /var/mail/boshy
yamadamasakinoMacBook-Pro:mywebapi boshy$ code .
yamadamasakinoMacBook-Pro:mywebapi boshy$ node index.js
Listening on port 3000