# PLL Take Home Backend

## Project Description

You are given the task to create a system architecture for a service to autogenerate a fantasy lacrosse team. You will be given sample JSON data that will contain information relevant for making decision on what players would make the best team.

### Project Setup
Install all the packages
Run `npm install`

To run the project run `npm run dev`

### Tasks

- [ ] Commit early and often. It is important to see your thought process. Act like you are collaborating with other engineers on the project.

- [ ] Implement folder structure to keep the files clean and easy to understand the purpose

- [ ] Create a system architecture design utilizing any AWS services for storing and fetching the data (No restrictions on a relational vs NoSql database, explain your reasoning for why you chose the services)

- [ ] Mock fetching the data from a database by using the sample fantasyPlayerInfo.json file

- [ ] Use the given information about the players to create a function that would auto generate the "best" team, not all fields are required. Explain your thought process on the "best" team

- [ ] Create REST API routes to save the generated team, get your saved team, and delete the team. Implement best practices for REST APIs

- [ ] Write a single unit test to test the team auto generating functions

### Relevant Info
#### Fantasy Team Criteria
1. The team must be under 200 salary cap
2. The fantasy team must have 2 Attack (A), 2 Midfield (M), 2 Defense (D, LSM, SSDM), 1 Goalie (G) positions
3. The team must fill all the positions, can’t be missing any positions
4. The outputted team will fit all the criteria and is expected to perform above average - Remember this is a functionality for a fan to use

###### Fantasy Stat Point Values
| Field Name | Point Value | 
| :-----------| :-----------: |
| onePointGoals | 10 points |
| twoPointGoals | 20 points |
| assists | 10 points |
| groundBalls | 1 points |
| causedTurnovers | 10 points |
| turnovers | -3 points |
| goalsAgainst | -1 points |
| twoPointGoalsAgainst | -2 points |
| saves | 3 points |
| faceoffsWon | .8 points |
| faceoffsLost | -1 points |

###### Stat Bonuses
If they have goals > 3

&nbsp;&nbsp;goalBonus: 5 points

If they have assists > 3

&nbsp;&nbsp;assistBonus: 5 points

If they have causedTurnovers > 3

&nbsp;&nbsp;causedTurnoverBonus: 5 points

If they have saves > 20

&nbsp;&nbsp;saveBonus: 5 points


### Testing
Use any testing framework that you prefer and setup the script to run the tests

### Submitting
Once you are finished, commit your changes and push them to your forked repo. Make sure to give access to the PLL github accounts to the repo so they can check it
