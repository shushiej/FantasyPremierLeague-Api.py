# FantasyPremierLeague-Api-Python

FantasyPremierLeague-Api-Python helps you access the data of the [Fantasy PremierLeague game] (https://fantasy.premierleague.com/). It is still a work in progress and is intended for use by people who want to get satistical data around the game for fun. For now, there is no API offered here, but a cool example where you can get interesting statistics about a certain league. Later on, I'll clean up the code and try to offer easy-to-use APIs.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine.

### Prerequisities

After cloning the project, you need to have the `requests` library on your machine. Run the following:

```
pip install requests
```

### Usage

For now, you can get 2 main things out of the python script:

* Distribution of players that are being picked in a specific League and GameWeek
* Distribution of players being captained in a specific League and GameWeek

Follow these easy steps to get these results for your league:

1. Go to [https://fantasy.premierleague.com/](https://fantasy.premierleague.com/) and login.
2. Go to leagues, and then click on the league you want to analyse
3. Check out the URL. It will be something like https://fantasy.premierleague.com/a/leagues/standings/**336217**/classic. Save the number, which is your league entry id.
4. Decide what GameWeek you want to analyse, let's say it's 2.
5. Run the following command at the root of your project: `python playersPickedInLeague.py --league 336217 --gameweek 2` or `python playersPickedInLeague.py -l 336217 -g 2`

Voila, you should be able to see 2 csv files created in the result folder.

### How to Contribute
This is just an example of what you can do with the fpl apis. I'm sure there are lots of cool ideas, so feel free to suggest by submitting an issue, or even write it yourself and send me a PR :)
