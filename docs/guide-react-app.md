# Creating a Github Pages React App


## Dependencies

The base packages needed are:

- Node
```text
$ node -v
v19.6.0
```
- npm/npx
```text
$ npm -v 
9.4.0
```
- git
```text 
$ git -v
git version 2.39.0.windows.1
``` 

With those packages we can proceed and install all other dependencies.

## Create an empty GitHub repository

## Create a React App

Using `npx` we can install and run the `create-react-app` tool. This action will create a new directory with the app name.

```bash
npx create-react-app nyaoka-app
```

## Install GitHub Pages node package 

This package will be a dev dependecy, this means that it is needed for development but the production version of the app won't use it.

```bash
cd nyaoka-app
npm install gh-pages --save-dev
```
## Configuration 

### Home Page

We need to setup a homepage for the app. In development this will be used set as `hebertluiz.github.io/nyaoka-site` and for final deployment will be `nyaoka.art.br`.



## Trobleshooting 

- Error during deploy
  - For the following error `fatal: a branch named 'gh-pages' already exists` you may need to remove the cached `gh-pages` node module with the following command `rm -rf node_modules/.cache/gh-pages`.

