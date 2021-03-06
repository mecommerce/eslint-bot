# Thirdlove Bot for PR! 

This bot is designed to run [eslint][] and [stylelint][] on any files modified by a pull-request, and post the results 
in a review comment.

### Initial Setup
  - Fork this repository and commit your `.eslintrc` files to the `config/` directory
  - presets may be added to `package.json: .dependencies`
  - nested files are supported so you can mirror your project structure: `config/test/.eslintrc.json` & 
    `config/.eslintrc.yml` will both apply.
  - Create a Heroku app and set the ENV vars detailed in [`example.env`](example.env) and the config.js file.
  - Create a new webhook on your github repository with:
    - Payload URL: `https://$YOUR_APP_NAME.herokuapp.com/run`
    - Content Type: `application/json`
    - Secret: `*****`
    - Events: `pull_request`

[eslint]: http://eslint.org
[stylelint]: https://stylelint.io/

### Heroku App

This is the [app][] in located under Thirdlove Heroku. You can find the logs [here]. 

Deploy the app by following these [steps][]. Use remote heroku and deploy in master. 

[app]: https://dashboard.heroku.com/apps/linter-bot/deploy/heroku-git
[here]: https://papertrailapp.com/systems/linter-bot/events
[steps]: https://dashboard.heroku.com/apps/linter-bot/deploy/heroku-git

# Thirdlove Bot TODO List

This file aims to contain a list of the missing features of the Thirdlove Bot. 
    
### Check the Backlog and fix one!

[Bot Backlog][https://github.com/mecommerce/eslint-bot/issues]

 
 
 
