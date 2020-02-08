# How to create angular cli and run on github pages

## Install Node and Npm on Mac
- open terminal
- run "brew update"
- run "brew install node"

## Install Angular CLI
- run "npm install -g @angular/cli"

## Create Github Repo
- Go to github.com and login
- Create new repo with your desired name

## Setup Github Pages
- go to settings -> githubpages -> set Master branch

## Clone Github Repo
- run "git clone [GITHUB CLONE LINK]"

## Create Angular Project
- navigate to clone repo and remove "Readme.md"
- navigate to parent folder of cloned repo "cd .."
- run "ng new [Name of the github repo]

## Install Github pages npm package
- run "npm install -g angular-cli-ghpages"

## Modify Output path in angular.json (under options)
- change "dist/[projectname]" to "dist/"

## Build project for pages
- run "ng build --prod --base-href FULLGITHUBPATH"
  - ex. ng build --prod --base-href https://bjmccotter7192/github.io/angularGitHubPages
- run "ngh"

## Change Github pages 
- Change the branch under settings -> githubpages -> gh-pages branch