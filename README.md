# fussball-de-matchplan-to-google-calendar
A match plan grabber for [fussball.de][0]

# Preparations

## Register application for Google calendar API

Go to [Google developer console][1], create a project to activate the calendar API. As platform choose webserver (node.js)
to access user data. Then create the client id. In the next step choose a product name to generate the client id etc. Then download the file in JSON format and store it in the application folder.

# Installation

## Arch Linux / Antergos
    sudo pacman -S nodejs npm git
    git clone https://github.com/BuZZ-dEE/fussball-de-matchplan-to-google-calendar.git
    cd fussball-de-matchplan-to-google-calendar
    sudo npm install -g

## NodeJS / NPM
    npm install -g fussball-de-matchplan-to-google-calendar

# Usage
    fussball-de-matchplan-to-google-calendar --team URL_TO_TEAM_NEXT_GAMES

e.g.

    fussball-de-matchplan-to-google-calendar --team http://www.fussball.de/ajax.team.next.games/-/team-id/01S687UBF8000000VS548985VUL18RL3

[0]: http://www.fussball.de/
[1]: https://console.developers.google.com/flows/enableapi?apiid=calendar
