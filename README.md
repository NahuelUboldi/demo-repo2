# deploy from react to ghpages
from the youtube video: [video](https://www.youtube.com/watch?v=M6hBd3Lomvw&t=467s)
## create a new repository in github
* from the plus icon in top right corner of the site
## commit changes in git
1. git status
1. git add .
1. git commit -m "text"
1. git remote add origin https://github.com/NahuelUboldi/awesome-markdown-previewer.git
1. git push -u origin master

## app to github pages
* download the package from: [package](https://www.npmjs.com/package/gh-pages)
  * npm i gh-pages

* add your project url to the package.json main props:
  * "homepage": "https://nahueluboldi.github.io/awesome-markdown-previewer/",
  
add this two lines to the script object inside the package.json file:
* "predeploy": "npm run build",
* "deploy": "gh-pages -d build",

## commit new changes in git
1. git status
1. git add .
1. git commit -m "gh-pages added"
1. git push

## deploy site
1. npm run deploy

## go to the site
* github -> settings -> github pages

#CREATE A REACT REDUX APP
* npx create-creact-app mi-app-name
* npm install redux react-redux
