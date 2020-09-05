# Deploying Node.js apps - The complete guide

## Solutins dicussed here
* Deploying to [**DPLYR**](https://www.dplyr.dev) 
* Deploying to Ubuntu 16.04 and above
* Deploying to AWS
* Deploying to Heroku

## Deploying to DPLYR
### You have two options when deploying to DPLYR either through the web dashboard or through the CLI tool
### Deploying from the CLI
> Note: You have to install Node.js and NPM 

* Run `npm i -g dplyr-cli` or with yarn `yarn global add dplyr-cli`

> If you face a permission issue when running the command above run the command line as an Adminstrator (Windows) or use sudo (MacOS and Linux)

* Run `dplyr auth` and enter the token you get from the [web dashboard](https://app.dplyr.dev) in the integrations panel, copy the API key and paste it in the CLI

* Run `dplyr deploy` in the root folder of your project it will ask you a couple of questions answer them all and proceed


## Deploying to Ubuntu 16 or above
* Run `sudo apt update`
* Run `sudo apt install git nodejs npm` 
* Clone your git project using `git clone GIT_PROJECT_URL`
* Inside your project folder run `npm install`
* While inside run `pm2 npm start npm`