# npm-sass-tutorial

## use npm to compile sass and watch for changes using scripts in package.json

### devDependencies
node-sass for sass
nodemon for watch changes

### install script
```
npm install --save-dev node-sass nodemon
```

### scripts
```
"scripts": {
  "build-css": "node-sass --include-path scss scss/main.scss public/css/main.css",
  "watch-css": "nodemon -e scss -x \"npm run build-css\""
}
```
