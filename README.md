# Flight_BOT


## Project Description
It is a slack bot developed in python in which user can run /slash commands. This project uses [OpenSky REST API](https://opensky-network.org/apidoc/rest.html).



## Installation

1. Clone the repository and navigate to `filght-bot` directory.
```
git clone https://github.com/vipin0/filght-bot.git
```
  
2. Install the required dependencies.
```
pip install -r requirements.txt
```
3. It's takes the following environment variables, create a file `.env` with the content of `.env.sample`.
```
SLACK_BOT_TOKEN=your-bot-token
SLACK_SIGNING_SECRET=your-signing-secret
PORT=4444
```
4. Start the development server.
```
python bot.py
```

## Available /[slash]commands
 - **/get_flights** *origin_code* *destination_code* *[YYYY-MM-DD]* *[no_passengers]* *[travel_class]*

 This command list all the flights between given airports on gievn date.

 You must provide origin airport code and destination airport code.<br>
    Default search date to today\'s date.<br>
    Default no_passengers is 1<br>
    Default travel_class is \'E\' or you can use \'B\'.

 - **/list_arrivals** *airport_code* *[begintime]* *[endtime]*

 This list all the flights arriving on the given airports.

 - **/list_departures** *airport_code* *[begintime]* *[endtime]*

 This list all the flights departing from the given airports.

 - **/help** 

 This command show the help menu for the bot.





