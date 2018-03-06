
# Slack Bot - Adding user in GitHub Organization and teams

This "Serverless" Slack bot is built with nodejs and StdLib. Some of the functions
and utilities were provided via StdLib´s quick guide to "Build a “Serverless” Slack Bot in 9 Minutes with Node.js and StdLib".

Link: <https://medium.com/slack-developer-blog/build-a-serverless-slack-bot-in-9-minutes-with-node-js-and-stdlib-b993cfa15358>

This slack bot can add a user to a team inside an organization. The user will first ask the bot for access to a specific repository by using slash-command. The user needs to provide a GitHub username and repository name. The bot will then post a message to a private admin channel where the admins can choose to give or denial the request. If they give access to the user, they will be prompted with which team they want to add the user into.


## Steps to add a user to a team on GitHub

The user need to write a slash-command named `ask`, for example: `/ask exampleUser repositoryName`
<img src="https://github.com/gissle-the-bot/test1/blob/master/preview-user-ask-command.png?raw=true" height="200" width="auto" >

He/she will then get a confirmation message that the request is sent to the admin channel:

<img src="https://github.com/gissle-the-bot/test1/blob/master/preview-user-request?raw=true" height="200" width="auto" >

The admin users will then be prompted with a give/denial access choice:

<img src="https://github.com/gissle-the-bot/test1/blob/master/preview-admin-give-access.png?raw=true" height="200" width="auto" >

If the admin user denial access to the user, they will be prompted with a "Access was not granted to ...." and the user will also receive a message. If the admin user give access, they will be prompted with a new message to choose team to add the user into:

<img src="https://github.com/gissle-the-bot/test1/blob/master/preview-admin-choose-team.png?raw=true" height="200" width="auto" >

After choosing team, the admins are done and will receive a summary message:

<img src="https://github.com/gissle-the-bot/test1/blob/master/preview-admin-summary.png?raw=true" height="auto" width="400" >

The user will receive a confirmation message:

<img src="https://github.com/gissle-the-bot/test1/blob/master/preview-user-respond.png?raw=true" height="auto" width="400" >

