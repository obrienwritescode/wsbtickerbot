# Reddit Mentioned Stocks Bot

Original credit goes to [RyanElliot10](https://github.com/RyanElliott10/wsbtickerbot)

## Overview

Reddit Mentioned Stocks Bot is a Reddit bot, developed utilizing the Reddit PRAW API, that scrapes the entirety of multiple subreddits over a 24 hour period, collects all the tickers mentioned, and then performs sentiment analysis on the context. The sentiment analysis is used to classify the stocks into three categories: bullish, neutral, and bearish. Once the list is complied the results are sent to a configured reddit users inbox.

## Setup

### Python Modules

```brew install python```

```pip3 install --upgrade pip```

```pip3 install praw```

```pip3 install Stock```

Ignore config.json file to never check in secrets

```git update-index --assume-unchanged config.json```

### Create Reddit app
1. Navigate to [apps](https://old.reddit.com/prefs/apps/)
2. Click create another app
3. Enter a Name
4. Enter redirect url which can be any URL
5. Copy the client id which is under the new app name to *client_id* in config.js
6. Copy secret to *client_secret* in config.js
7. Update *username* with your Reddit username in config.js
8. Update *password* with your Reddit password in config.js
9. Update *DestinationUsername* to the user you wish to send the message

### Create IEX Cloud account
1. Create a free API account with [IEX Cloud](https://iexcloud.io/)
2. Update *iex_apikey* in config.js
