# deploy from react to ghpages
from the youtube video: [https://www.youtube.com/watch?v=M6hBd3Lomvw&t=467s](https://www.youtube.com/watch?v=M6hBd3Lomvw&t=467s)
## create a new repository in github
- from the plus icon in top right corner of the site
## commit changes in git
- git status
- git add .
- git commit -m "text"
- git remote add origin https://github.com/NahuelUboldi/awesome-markdown-previewer.git
- git push -u origin master

## app to github pages
- download the package from: [https://www.npmjs.com/package/gh-pages](https://www.npmjs.com/package/gh-pages)
  - npm i gh-pages

- add your project url to the package.json main props:
  - "homepage": "https://nahueluboldi.github.io/awesome-markdown-previewer/",
  
add this two lines to the script object inside the package.json file:
- "predeploy": "npm run build",
- "deploy": "gh-pages -d build",

## commit new changes in git
- git status
- git add .
- git commit -m "gh-pages added"
- git push

## deploy site
- npm run deploy

## go to the site
- github -> settings -> github pages

