# npm-sass-tutorial

## use npm to compile sass and watch for changes using scripts in package.json

### devDependencies
1. **node-sass** for sass,
2. **nodemon** for watch changes

### install script
```
npm install --save-dev node-sass nodemon
```

### scripts: paths follow *--include-path will need to be changed*
```
"scripts": {
  "build-css": "node-sass --include-path scss scss/main.scss public/css/main.css",
  "watch-css": "nodemon -e scss -x \"npm run build-css\""
}
```
