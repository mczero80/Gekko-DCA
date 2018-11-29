# Gekko (Dollar Cost Average) Bot

If you want the original Gekko Trading Bot, go here:
https://github.com/askmike/gekko

I modded the Gekko Trading Bot to Dollar Cost Average (NOTE: The bot no longer works as a trading bot, if you want to have the DCA bot and Trading bot on the same machine, you need to have them installed on separate folders). To be honest, I only made minor changes to the bot to get it to work this way. The bot works quite well already so all I had to do was modify 3 files (check the commit to see which files were changed) and add the dollar cost average strategy. To get this bot to work, install the same way you would Gekko, and then do the following:

1. Make a copy or rename the config file "sample-config.js" (Ex: config-live.js or config-BTC-live.js).
2. In the config file, under config.DCA, adjust how often you want Gekko to Dollar Cost Average buy. 
3. Put in your exchange API key in the config.trader section and scroll to the end of the file and confirm you are responsible for your own strategies and that Gekko only automates it for you. 
3. Go to /plugins/trader/trader.js, modify the dcaAmount variable to adjust how much currency to use to buy during each interval.
4. Start the bot by going to Gekko folder in Terminal or Command Prompt and type in node gekko.js --config config-live.js (or whatever you named the config file to).

_________________________________________________________________________________

![Gordon Gekko](http://mikevanrossum.nl/static/gekko.jpg)

*The most valuable commodity I know of is information.*

-Gordon Gekko

Gekko is a Bitcoin TA trading and backtesting platform that connects to popular Bitcoin exchanges. It is written in JavaScript and runs on [Node.js](http://nodejs.org).

*Use Gekko at your own risk.*

## Documentation

See [the documentation website](https://gekko.wizb.it/docs/introduction/about_gekko.html).

## Installation & Usage

See [the installing Gekko doc](https://gekko.wizb.it/docs/installation/installing_gekko.html).

## Community & Support

Gekko has [a forum](https://forum.gekko.wizb.it/) that is the place for discussions on using Gekko, automated trading and exchanges. In case you rather want to chat in realtime about Gekko feel free to join the [Gekko Support Discord](https://discord.gg/26wMygt).

## Final

If Gekko helped you in any way, you can always leave me a tip at (BTC) 13r1jyivitShUiv9FJvjLH7Nh1ZZptumwW
