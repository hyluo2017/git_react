
# project setup
$ npx create-react-app . (create react app at root .)
$ npm i gh-pages (install gh-pages - a node module, this will create node_modeules folder)
in package.json, add:
    "homepage": "https://hyluo2017.github.io/n2tnotes",
    in "scripts" add: "deploy": "gh-pages -d dist"
create .gitignore file

# git local
$ git init (create a .git folder)
$ git add . (add everything to staging)
$ git commit -m "any comment" 

# push to github.com
(ref: https://github.com/hyluo2017/n2tnotes)
$ git branch -M main  (name of repo branch! can also by 'master'? but consistent below)
$ git remote add origin https://github.com/hyluo2017/n2tnotes.git
$ git push -u origin main

# deploy
(since now there is only main branch, not gh-pages branch)
$ npm run deploy
Published!

# check it out
ref: https://github.com/hyluo2017/n2tnotes/settings/pages
 Your site is published at https://hyluo2017.github.io/n2tnotes/

# link to owned domain name:
12'05-15'