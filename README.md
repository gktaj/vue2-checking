# vue2-checking
This project was built by Vue 3.2.1.

## Local environment
```
$ git clone https://github.com/kdevsoftware/vue2-checking.git
$ cd vue2-checking
$ npm install
$ npm run serve
```
Navigate to `http://localhost:8080/`.

## Deploying to github page
```
$ npm run deploy
```
Navigate to `https://kdevsoftware.github.io/vue2-checking/`.

## Reference for deploying to github page

### 1. Install vue-gh-pages package
```
$ npm install --save-dev vue-gh-pages
```

### 2. Add "deploy" script to package.json
```
"scripts": {
  ...  
  "deploy": "node ./node_modules/vue-gh-pages/index.js --branch gh-pages"
  ...
```

### 3. Add "homepage" field to package.json
```
"homepage": "https://github.com/kdevsoftware/vue2-checking",
"scripts": {
  ...
```

### 4. Deploy to github
```
$ npm run deploy
```
Navigate to `https://kdevsoftware.github.io/vue2-checking/`.