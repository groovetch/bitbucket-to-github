## Bitbucket to Github Migration
This repository transfers ALL of your Bitbucket repositories to Github while maintaining its privacy status.
### Getting Started
Make sure you have node and npm before continuing. Make sure 2FA features were disabled for both github and bitbucket
##### Clone the repo
`git clone git@github.com:groovetch/bitbucket-to-github.git`
##### Enter the repo
`cd bitbucket-to-github/`
##### Install dependencies
`npm i` or `yarn`
##### Make an environment variable file
`cp .env.sample .env`
##### Create an access token on Github
Use `https://help.github.com/articles/creating-a-personal-access-token-for-the-command-line/` to create your token.
##### Enter your Github and Bitbucket credentials to `.env`
This repository uses the `dotenv` library to handle configuration variables. 
It should be noted that the Bitbucket 'username' is not your email address but 'https://bitbucket.org/{username}/{repo_name}'
It should also be noted that the Github token requires full repo permissions if you want to create private repositories.
##### Run the script
`node index.js`

