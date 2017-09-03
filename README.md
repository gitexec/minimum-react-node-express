# minimum-react-node-express

This is a basic configuration app for the client and server side using react and node with express. Kudo to the source below

STEPS

* npm init -y

* npm install --save express morgan

=== React Related ===

* npm install --save react react-dom

* npm install --save-dev babel-core babel-loader babel-preset-react babel-preset-stage-0 babel-cli babel-preset-es2015 rimraf


* in root directory vim .babelrc

* add to .babelrc

{

  "presets": ["es2015", "stage-0", "react"]

}

* Add under scripts:

"build": "rimraf dist/ && babel ./ --out-dir dist/ --ignore ./node_modules,./.babelrc,./package.json,./npm-debug.log --copy-files",

"start": "npm run build && node dist/index.js"

Push to your github:

* echo node_modules > .gitignore

git init

git add README.md

git commit -m "first commit"

git remote add origin https://github.com/KAMEKAMEKAME

git push -u origin master

source: https://www.codementor.io/iykyvic/writing-your-nodejs-apps-using-es6-6dh0edw2o#comments-6dh0edw2o

and 

https://stackoverflow.com/questions/33460420/babel-loader-jsx-syntaxerror-unexpected-token

