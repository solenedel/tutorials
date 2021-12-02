# Deploying to GitHub Pages with your own react app (no templates)

## Tutorial link: https://www.youtube.com/watch?v=F8s4Ng-re0E

### 1. create react app locally

`npx create-react-app my-app`

### 2. on GitHub, create a new repository with the same name as the react app you just created. No Readme is needed.


### 3. in VScode, run the following command:
  `npm install gh-pages --save-dev`

### 4. Go to package.json and add a few lines:

**At the very top:**
```
"homepage": "http://username.github.io/my-app",
```
The pattern is github-username.github.io/repo-name

Also make sure that gh-pages is listed as a dependency at the bottom of the file.

**in the "scripts" section, add:**

```
"predeploy": "npm run build",
"deploy": "gh-pages -d build",
```


### 5. On your local machine, run these commands inside the project folder.

`git init`
`git remote add origin git@github.com:solenedel/blog.git`

### 6. Make some changes locally, then `git add .` and `git commit`

### 7. Run `npm run deploy`

### 8. Push to github: `git push -u origin main`

### 9. on GitHub, go to the repository page and go to settings > pages.

It should say that the app is deployed and give the link to the deployed page. 




## Note: images should be inside the src folder 