# An [OpenWeatherMap](https://openweathermap.org/api) bot for Slack in NodeJS 
This is a bot for delivering real-time weather information from OpenWeatherMap built on Slack's NodeJS SDK using:
- [Web](https://api.slack.com/web) API
- [Real Time Messaging (RTM)](https://api.slack.com/rtm) API
- [Events](https://api.slack.com/events-api) API
- [Node Slack SDK](https://github.com/slackapi/node-slack-sdk)

## Installation
### Set up the Slack bot-user
Slack requires you to add a bot configuration to your workspace. Head to
[**_your-workspace-name_**.slack.com/apps/A0F7YS25R-bots](https://slack.com/apps/A0F7YS25R-bots)
and add a new configuration.

Alternatively, you can:
1. go to your workspace settings at **_your-workspace-name_**.slack.com/**apps/manage**
2. search for the 'Bots' app and add a new configuration to your workspace

![alt text](https://i.imgur.com/QuwB4M1.gif "Search and add")

**NOTE**: Keep your bot secret-token handy and secret for later- it is necessary for connecting to the Slack client

### NodeJS & npm
You will want to grab the latest NodeJS/npm.
After installation and verifying you have the latest version, you can create a new folder, **clone the repository**, and run your `npm install` to grab the dependencies.

### OWM API Key
Head to [OpenWeatherMap](https://openweathermap.org/appid) and sign up for current weather data.
Keep the API key handy (in addition to the Slack bot key mentioned previously); you will need it when setting up your enviornment variables in the next step.
(The OWM-API docs also provide great information on how to further use the API).

### Setting up the envrionment variables
After the repository has been cloned, NodeJS and npm updated, and dependency modules installed, the last step is to place your secret keys into the environment variables.
Create a new file `.env` and add the following lines of text:
```
SLACK_BOT_TOKEN=<SECRET KEY HERE>
OWM_API_KEY=<OWM API KEY GOES HERE>
```

You can proceed to proceed to start the application with `node app.js`

## Usage
There are two main ways to interact with the bot: either through 



