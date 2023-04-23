# FRC Countdown Clock
The FRC Countdown Clock is a useful tool for teams participating in the FIRST Robotics Competition. It provides a countdown to the team's next match, ensuring that everyone is aware of the timing and can be properly prepared. The program generates a web page displaying information related to a specific FIRST Robotics Competition  team's participation in an event. The page displays a countdown to the team's next match, a table showing the team's matches and opponents, a panel with information on the team's next match and current match, and a panel with the team's current status in the competition.

## Features
Displays the time remaining until the team's next match\
Updates automatically based on the current time and match schedule\
Configurable to account for breaks and delays in the competition schedule\

## Usage
To use the FRC Countdown Clock, follow these steps:

Download the source code from the GitHub repository.\
Customize the configuration file to match your team's schedule and preferences.\
Build the code using your preferred development environment.\
Run the application on a device of your choice, such as a laptop or tablet.\
Display the countdown clock in a prominent location where everyone on the team can see it.

## Configuration
The success.php file includes the following options:

The `getRankings()` function retrieves the current rankings of teams participating in the event from The Blue Alliance API and saves them to a global variable for later use.

The `getMatches()` function retrieves information on the matches in which the team is participating from The Blue Alliance API and saves them to a global variable for later use. This includes the match number, the teams competing in the match, and the predicted start time of the match.

The `getMatchTypes()` function categorizes the matches into their respective types (practice, qualification, or elimination) and saves them to a global variable for later use.

The `sortMatches()` function sorts the matches by their start time in ascending order and saves them to a global variable for later use.

The `countDown()` function retrieves the team's next match from the sorted matches and returns a formatted countdown to the predicted start time of the match.

The `getCurrentMatch()` function retrieves information on the team's current match from The Blue Alliance API and saves the match number to a global variable for later use.

The `virtualKettering()` function generates an HTML table displaying the team's matches and opponents. The table includes the match number, the teams competing in the match, their rankings, and the predicted start time of the match.

The `getNextMatch()` function retrieves the team's next match from the sorted matches and saves it to a global variable for later use.

The `nextMatchPanel()` function generates an HTML panel displaying information on the team's next match and current match. The panel includes the match number, the teams competing in the match, the team's bumper color, and the current match number.

The `statusPanel()` function generates an HTML panel displaying the team's current status in the competition. The panel includes the team's current rank, record, and playoff status.
