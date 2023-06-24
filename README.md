# nucamp_devops_project

Portfolio Project Report - Week 1
Project: Basketball Team and Player Management Application

**Features:**
The basketball team and player management application will offer the following features:

a) Team Management:
Create a new basketball team.
Retrieve a specific basketball team.
Update the information of a basketball team.
Delete a basketball team.

b) Player Management:
Add a new player to a basketball team.
Retrieve a specific player.
Update the information of a player.
Delete a player.

**API Endpoints:**
a) Team Management Endpoints:
Create a new basketball team:

**HTTP Verb: POST**
Endpoint URL: /teams/
Special Details: Request body should contain the team's information (team name, coach name).
Retrieve a specific basketball team:

**HTTP Verb: GET**
Endpoint URL: /teams/{team_id}/
Special Details: The team_id parameter represents the unique identifier of the basketball team.
Update the information of a basketball team:

**HTTP Verb: PUT/PATCH**
Endpoint URL: /teams/{team_id}/
Special Details: The team_id parameter represents the unique identifier of the basketball team. The request body should contain the updated team information.
Delete a basketball team:

**HTTP Verb: DELETE**
Endpoint URL: /teams/{team_id}/
Special Details: The team_id parameter represents the unique identifier of the basketball team.
b) Player Management Endpoints:

Add a new player to a basketball team:

**HTTP Verb: POST**
Endpoint URL: /teams/{team_id}/players/
Special Details: The team_id parameter represents the unique identifier of the basketball team. The request body should contain the player's information (player name, position, height, weight).
Retrieve a specific player:

**HTTP Verb: GET**
Endpoint URL: /players/{player_id}/
Special Details: The player_id parameter represents the unique identifier of the player.
Update the information of a player:

**HTTP Verb: PUT/PATCH**
Endpoint URL: /players/{player_id}/
Special Details: The player_id parameter represents the unique identifier of the player. The request body should contain the updated player information.
Delete a player:

**HTTP Verb: DELETE**
Endpoint URL: /players/{player_id}/
Special Details: The player_id parameter represents the unique identifier of the player.
Database Tables:
Database Name: basketball_app_db

**Table: Team**
Columns:
id (Primary Key, Integer)
team_name (String)
coach_name (String)

**Table: Player**
Columns:
id (Primary Key, Integer)
team_id (Foreign Key referencing Team.id)
player_name (String)
position (String)
height (Float)
weight (Float)

**Constraints:**
Team.id: Primary Key constraint.
Player.id: Primary Key constraint.
Player.team_id: Foreign Key constraint referencing Team.id.
