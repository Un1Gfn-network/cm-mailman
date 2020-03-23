[Original post](https://blog.jan-ahrens.eu/2014/06/17/heroku-with-c.html)  
[Original repo](https://github.com/JanAhrens/ipconfig-http-server)

```
$ g remote add heroku https://git.heroku.com/cybermusketeers.git
```

```
$ p -u heroku master
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 2 threads
Compressing objects: 100% (7/7), done.
Writing objects: 100% (8/8), 5.20 KiB | 2.60 MiB/s, done.
Total 8 (delta 0), reused 0 (delta 0)
remote: Compressing source files... done.
remote: Building source:
remote: 
remote: -----> Node.js app detected
remote:        
remote: -----> Creating runtime environment
remote:        
remote:        NPM_CONFIG_LOGLEVEL=error
remote:        NODE_ENV=production
remote:        NODE_MODULES_CACHE=true
remote:        NODE_VERBOSE=false
remote:        
remote: -----> Installing binaries
remote:        engines.node (package.json):  unspecified
remote:        engines.npm (package.json):   unspecified (use default)
remote:        
remote:        Resolving node version 12.x...
remote:        Downloading and installing node 12.16.1...
remote:        Using default npm version: 6.13.4
remote:        
remote: -----> Installing dependencies
remote:        Installing node modules (package.json)
remote:        up to date in 0.262s
remote:        found 0 vulnerabilities
remote:        
remote:        
remote: -----> Build
remote:        
remote: -----> Caching build
remote:        - node_modules (nothing to cache)
remote:        
remote: -----> Pruning devDependencies
remote:        up to date in 0.324s
remote:        found 0 vulnerabilities
remote:        
remote:        
remote: -----> Build succeeded!
remote: -----> Discovering process types
remote:        Procfile declares types -> web
remote: 
remote: -----> Compressing...
remote:        Done: 22.1M
remote: -----> Launching...
remote:        Released v3
remote:        https://cybermusketeers.herokuapp.com/ deployed to Heroku
remote: 
remote: Verifying deploy... done.
To https://git.heroku.com/cybermusketeers.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'heroku'.
```

```
curl -x "socks5h://127.0.0.1:1080" http://un1gfn.herokuapp.com/
```
