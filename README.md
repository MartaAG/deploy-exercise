This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

A simple exercise on deploying a react-app on github pages.
I based on two tutorials:

[How to deploy a Create React App Website to GitHub Pages by Programming Liftoff](https://www.youtube.com/watch?v=ctLFWAanxcI&list=PL4MuKcZFqNDKOw-f-rOPTlICcqauQ58nS&index=2&t=0s)

[How to Deploy React App to GitHub Pages by Telmo Sampaio](https://www.youtube.com/watch?v=F8s4Ng-re0E&list=PL4MuKcZFqNDKOw-f-rOPTlICcqauQ58nS&index=3&t=0s)

### `create-react-app`

First, create your app in create-react-app

### create a new repository on [GitHub](www.github.com)
And then push the project to the Github.
Go to Settings -> Github Pages -> source: 'master branch'
This way we can get the URL of our project. Copy it
### `npm install gh-pages --save-dev`.
You should have information in your package.json if github pages installed properly.
"devDependencies": {
  "gh-pages": "version"
}
### Open package.json

  Write it in convenient places:
  `"homepage": "URL taken from second step"
  "scripts": {
    "predeploy": "npm run build",
    "deploy": "gh-pages -d build"
  }
  `

### Commit your changes

### `npm run deploy`

It may take few minutes. It may be a possibility that you will be asked for your password.

### Go back to your project settings on your Github
Settings -> GitHub Pages -> Source -> (after refresh) gh-pages branch.

### open the link which Github pages generated.
After few minutes the webpage is deployed. The changes made in local files are visible in the webpage. 
