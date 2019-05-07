# ![LOGO](logo.png) NFL v3 Stats **flow**ground Connector

## Description

A generated **flow**ground connector for the NFL v3 Stats API (version 1.0).

Generated from: https://api.apis.guru/v2/specs/fantasydata.net/nfl-v3-stats/1.0/swagger.json<br/>
Generated at: 2019-05-07T17:40:38+03:00

## API Description

NFL rosters, player stats, team stats, and fantasy stats API.

## Authorization

Supported authorization schemes:
- API Key- API Key
## Actions

### Legacy Box Scores Active

> This method returns box scores for all games that are either in-progress or have been updated within the last 30 minutes.

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.

### Teams (All)

> Gets all teams, including pro bowl teams.

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.

### Are Games In Progress

> Returns <code>true</code> if there is at least one game being played at the time of the request or <code>false</code> if there are none.

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.

### Legacy Box Score

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - 
          Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        
* `week` - _required_ - 
          Week of the season. Valid values are as follows: Preseason 0 to 4, Regular Season 1 to 17, Postseason 1 to 4.
          Example: <code>1</code>
        
* `hometeam` - _required_ - Abbreviation of the home team. Example: <code>WAS</code>.

### Box Score by ScoreID V3

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `scoreid` - _required_ - The ScoreID of the game. Possible values include: <code>16247</code>, <code>16245</code>, etc.

### Box Score V3

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        
* `week` - _required_ - Week of the season. Valid values are as follows: Preseason 0 to 4, Regular Season 1 to 17, Postseason 1 to 4.
          Example: <code>1</code>
        
* `hometeam` - _required_ - Abbreviation of a team playing in this game. Example: <code>WAS</code>.

### Legacy Box Scores

> This method returns all box scores for a given season and week.

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - 
          Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        
* `week` - _required_ - 
          Week of the season. Valid values are as follows: Preseason 0 to 4, Regular Season 1 to 17, Postseason 1 to 4.
          Example: <code>1</code>
        

### Legacy Box Scores Delta

> This method returns all box scores for a given season and week, but only returns player stats that have changed in the last X minutes.

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        
* `week` - _required_ - Week of the season. Valid values are as follows: Preseason 0 to 4, Regular Season 1 to 17, Postseason 1 to 4.
          Example: <code>1</code>
        
* `minutes` - _required_ - Only returns player statistics that have changed in the last X minutes.  You specify how many minutes in time to go back.  Valid entries are:<br>
          <code>1</code> or <code>2</code>.
        

### Box Scores Delta V3

> This method returns all box scores for a given season and week, but only returns player stats that have changed in the last X minutes. You can also filter by type of player stats to include, such as traditional fantasy players, IDP players or all players.

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        
* `week` - _required_ - Week of the season. Valid values are as follows: Preseason 0 to 4, Regular Season 1 to 17, Postseason 1 to 4.
          Example: <code>1</code>
        
* `playerstoinclude` - _required_ - The subcategory of players to include in the returned PlayerGame records. Possible values include:<br><br>
<code>all</code> Returns all players<br>
<code>fantasy</code> Returns traditional fantasy players (QB, RB, WR, TE, K, DST)<br>
<code>idp</code> Returns traditional fantasy players and IDP players.
    Possible values: all, fantasy, idp.
* `minutes` - _required_ - Only returns player statistics that have changed in the last X minutes.  You specify how many minutes in time to go back.  Valid entries are:<br><code>1</code>,
 <code>2</code>, etc.
        

### Bye Weeks

> Get bye weeks for the teams during a specified NFL season.

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
* `season` - _required_ - 
          Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        

### Season Current

> Year of the current NFL season. This value changes on July 1st. The earliest season for Fantasy data is 2001. The earliest season for Team data is 1985. The earliest season for Fantasy data is 2001. The earliest season for Team data is 1985.

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.

### Week Current

> Number of the current week of the NFL season. This value usually changes on Tuesday nights or Wednesday mornings at midnight EST. Week number is an integer between 1 and 21 or the word current. Weeks 1 through 17 are regular season weeks. Weeks 18 through 21 are post-season weeks.

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.

### Daily Fantasy Players

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `date` - _required_ - 
          The date of the contest for which you're pulling players
          <code>2014-SEP-21</code>,
          <code>2014-NOV-15</code>, etc
        

### Daily Fantasy Scoring

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `date` - _required_ - The date of the contest for which you're pulling players
          <code>2014-SEP-21</code>,
          <code>2014-NOV-15</code>, etc

### DFS Slates by Date

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `date` - _required_ - The date of the slates.
<br>Examples: <code>2017-SEP-25</code>, <code>2017-10-31</code>.

### DFS Slates by Week

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        
* `week` - _required_ - Week of the season. Valid values are as follows: Preseason 0 to 4, Regular Season 1 to 17, Postseason 1 to 4.
          Example: <code>1</code>
        

### Fantasy Defense Game Stats

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - 
          Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        
* `week` - _required_ - 
          Week of the season. Valid values are as follows: Preseason 0 to 4, Regular Season 1 to 17, Postseason 1 to 4.
          Example: <code>1</code>
        

### Fantasy Defense Game Stats by Team

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        
* `week` - _required_ - Week of the season. Valid values are as follows: Preseason 0 to 4, Regular Season 1 to 17, Postseason 1 to 4.
          Example: <code>1</code>
        
* `team` - _required_ - Abbreviation of the team. Example: <code>WAS</code>.

### Fantasy Defense Season Stats

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - 
          Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        

### Fantasy Defense Season Stats by Team

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        
* `team` - _required_ - Abbreviation of the team. Example: <code>WAS</code>.

### Fantasy Players with ADP

> This method returns a comprehensive list of draftable fantasy football players, including QB, RB, WR, TE, K and DEF.  Players are sorted by ADP (AverageDraftPosition).

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.

### IDP Fantasy Players with ADP

> This method returns the top 300+ IDP Fantasy Players for the current or upcoming season, ordered by AverageDraftPositionIDP.

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.

### Legacy Box Scores Final

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.

### Player Details by Free Agents

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.

### League Leaders by Week

#### Input Parameters
* `format` - _required_ - 
          Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
        
    Possible values: XML, JSON.
* `season` - _required_ - 
          Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        
* `week` - _required_ - 
          Week of the season. Valid values are as follows: Preseason 0 to 4, Regular Season 1 to 17, Postseason 1 to 4.
          Example: <code>1</code>
        
* `position` - _required_ - PlayeraEU(tm)s position that you would like to filter by.
    Possible values: ALL, OFFENSE, QB, RB, WR, TE, DEFENSE, DL, LB, DB, K.
* `column` - _required_ - Response member you would like results sorted by.
    Possible values: FantasyPoints, PassingYards, RushingYards, Receptions, Sacks, Interceptions, Touchdowns.

### Game Stats by Season (Deprecated, use Team Game Stats instead)

> Game stats for a specified season.

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - 
          Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        

### Game Stats by Week (Deprecated, use Team Game Stats instead)

> Game stats for a specified season and week.

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - 
          Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        
* `week` - _required_ - 
          Week of the season. Valid values are as follows: Preseason 0 to 4, Regular Season 1 to 17, Postseason 1 to 4.
          Example: <code>1</code>
        

### Injuries

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - 
          Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        
* `week` - _required_ - 
          Week of the season. Valid values are as follows: Preseason 0 to 4, Regular Season 1 to 17, Postseason 1 to 4.
          Example: <code>1</code>
        

### Injuries by Team

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - 
          Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        
* `week` - _required_ - 
          Week of the season. Valid values are as follows: Preseason 0 to 4, Regular Season 1 to 17, Postseason 1 to 4.
          Example: <code>1</code>
        
* `team` - _required_ - Abbreviation of the team. Example: <code>WAS</code>.

### Season Last Completed

> Year of the most recently completed season. this value changes immediately after the Super Bowl. The earliest season for Fantasy data is 2001. The earliest season for Team data is 1985.

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.

### Week Last Completed

> Number of the last completed week in the current NFL season. This value changes immediately after the last game of the week is completed and the data is available. This usually happens right after the Monday night game.<br/>
>         Week number is an integer between 1 and 21 or the word current. Weeks 1 through 17 are regular season weeks. Weeks 18 through 21 are post-season weeks.

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.

### Legacy Box Scores Live

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.

### News

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.

### News by Date

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
* `date` - _required_ - The date of the news.
<br>Examples: <code>2017-JUL-31</code>, <code>2017-SEP-01</code>.

### News by Player

#### Input Parameters
* `format` - _required_ - 
          Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
        
* `playerid` - _required_ - Each NFL player has a unique ID assigned by FantasyData. Player IDs can be determined by pulling player related data. Example:<code>14257</code>.

### News by Team

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
* `team` - _required_ - Abbreviation of the team. Example: <code>WAS</code>.

### Player Details by Player

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `playerid` - _required_ - Each NFL player has a unique ID assigned by FantasyData. Player IDs can be determined by pulling player related data. Example:<code>732</code>.

### Player Game Red Zone Stats Inside Five

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        
* `week` - _required_ - Week of the season. Valid values are as follows: Preseason 0 to 4, Regular Season 1 to 17, Postseason 1 to 4.
          Example: <code>1</code>
        

### Player Game Red Zone Stats Inside Ten

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        
* `week` - _required_ - Week of the season. Valid values are as follows: Preseason 0 to 4, Regular Season 1 to 17, Postseason 1 to 4.
          Example: <code>1</code>
        

### Player Game Red Zone Stats

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        
* `week` - _required_ - Week of the season. Valid values are as follows: Preseason 0 to 4, Regular Season 1 to 17, Postseason 1 to 4.
          Example: <code>1</code>
        

### Player Game Stats by Player

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - 
          Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        
* `week` - _required_ - 
          Week of the season. Valid values are as follows: Preseason 0 to 4, Regular Season 1 to 17, Postseason 1 to 4.
          Example: <code>1</code>
        
* `playerid` - _required_ - Each NFL player has a unique ID assigned by FantasyData. Player IDs can be determined by pulling player related data. Example:<code>732</code>.

### Player Game Stats by Team

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - 
          Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        
* `week` - _required_ - 
          Week of the season. Valid values are as follows: Preseason 0 to 4, Regular Season 1 to 17, Postseason 1 to 4.
          Example: <code>1</code>
        
* `team` - _required_ - Abbreviation of the team. Example: <code>WAS</code>.

### Player Game Stats by Week

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - 
          Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        
* `week` - _required_ - 
          Week of the season. Valid values are as follows: Preseason 0 to 4, Regular Season 1 to 17, Postseason 1 to 4.
          Example: <code>1</code>
        

### Player Game Stats by Week Delta

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - 
          Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        
* `week` - _required_ - 
          Week of the season. Valid values are as follows: Preseason 0 to 4, Regular Season 1 to 17, Postseason 1 to 4.
          Example: <code>1</code>
        
* `minutes` - _required_ - Only returns player statistics that have changed in the last X minutes.  You specify how many minutes in time to go back.  Valid entries are:<br>
          <code>1</code> or <code>2</code>.
        

### Player Game Stats Delta

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `minutes` - _required_ - 
          Only returns player statistics that have changed in the last X minutes.  You specify how many minutes in time to go back.  Valid entries are:
          <code>1</code> or <code>2</code>.
        

### Fantasy Player Ownership Percentages (Season-Long)

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        
* `week` - _required_ - Week of the season. Valid values are as follows: Preseason 0 to 4, Regular Season 1 to 17, Postseason 1 to 4.
          Example: <code>1</code>
        

### Player Season Red Zone Stats Inside Five

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        

### Player Season Red Zone Stats Inside Ten

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        

### Player Season Red Zone Stats

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        

### Player Season Stats

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - 
          Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        

### Player Season Stats by Player

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - 
          Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        
* `playerid` - _required_ - Each NFL player has a unique ID assigned by FantasyData. Player IDs can be determined by pulling player related data. Example:<code>732</code>.

### Player Season Stats by Team

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - 
          Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        
* `team` - _required_ - Abbreviation of the team. Example: <code>WAS</code>.

### Player Season Third Down Stats

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - 
          Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        

### Player Details by Available

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.

### Player Details by Team

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `team` - _required_ - Abbreviation of the team. Example: <code>WAS</code>.

### Pro Bowlers

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - Year of the season
<br>Examples: <code>2016</code>, <code>2017</code>

### Legacy Box Scores Delta (Current Week)

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `minutes` - _required_ - Only returns player statistics that have changed in the last X minutes.  You specify how many minutes in time to go back.  Valid entries are:<br>
          <code>1</code> or <code>2</code>.
        

### Player Details by Rookie Draft Year

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
* `season` - _required_ - Year of the season.<br>Examples: <code>2018</code>, <code>2019</code>, etc.

### Schedule

> Game schedule for a specified season.

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
* `season` - _required_ - Year of the season (with optional season type).<br>Examples: <code>2018</code>, <code>2018PRE</code>, <code>2018POST</code>, <code>2018STAR</code>, <code>2019</code>, etc.

### Scores by Season

> Game scores for a specified season.

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
* `season` - _required_ - Year of the season (with optional season type).<br>Examples: <code>2018</code>, <code>2018PRE</code>, <code>2018POST</code>, <code>2018STAR</code>, <code>2019</code>, etc.

### Scores by Week

> Get game scores for a specified week of a season.

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
* `season` - _required_ - 
          Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        
* `week` - _required_ - 
          Week of the season. Valid values are as follows: Preseason 0 to 4, Regular Season 1 to 17, Postseason 1 to 4.
          Example: <code>1</code>
        

### League Leaders by Season

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - 
          Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        
* `position` - _required_ - PlayeraEU(tm)s position that you would like to filter by.
    Possible values: ALL, OFFENSE, QB, RB, WR, TE, DEFENSE, DL, LB, DB, K.
* `column` - _required_ - Response member you would like results sorted by.
    Possible values: FantasyPoints, PassingYards, RushingYards, Receptions, Sacks, Interceptions, Touchdowns.

### Box Scores V3 Simulation

> Gets simulated live box scores of NFL games, covering the Conference Championship games on January 21, 2018.

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `numberofplays` - _required_ - The number of plays to progress in this NFL live game simulation. Example entries are <code>0</code>, <code>1</code>, <code>2</code>, <code>3</code>, <code>150</code>, <code>200</code>, etc.

### Scores by Week Simulation

> Gets simulated live scores of NFL games, covering the Conference Championship games on January 21, 2018.

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `numberofplays` - _required_ - The number of plays to progress in this NFL live game simulation. Example entries are <code>0</code>, <code>1</code>, <code>2</code>, <code>3</code>, <code>150</code>, <code>200</code>, etc.

### Stadiums

> This method returns all stadiums.

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.

### Standings

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
* `season` - _required_ - 
          Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        

### Team Game Stats

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - 
          Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        
* `week` - _required_ - 
          Week of the season. Valid values are as follows: Preseason 0 to 4, Regular Season 1 to 17, Postseason 1 to 4.
          Example: <code>1</code>
        

### Team Season Stats

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
    Possible values: XML, JSON.
* `season` - _required_ - 
          Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        

### Teams (Active)

> Gets all active teams.

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.

### Teams by Season

> List of teams playing in a specified season.

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
* `season` - _required_ - 
          Year of the season and the season type. If no season type is provided, then the default is regular season.
          <br>Examples: <code>2015REG</code>, <code>2015PRE</code>, <code>2015POST</code>.
        

### Timeframes

> Get detailed information about past, present, and future timeframes.

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.
* `type` - _required_ - The type of timeframes to return.  Valid entries are <code>current</code> or <code>upcoming</code> or <code>completed</code> or <code>recent</code> or <code>all</code>.

### Season Upcoming

> Year of the current NFL season, if we are in the mid-season. If we are in the off-season, then year of the next upcoming season. This value changes immediately after the Super Bowl. The earliest season for Fantasy data is 2001. The earliest season for Team data is 1985.

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.

### Week Upcoming

> Number of the upcoming week of the NFL season. This value changes immediately after the final game of the week is completed. We consider upcoming week to be the current week, until current week is over. Week number is an integer between 1 and 21 or the word current. Weeks 1 through 17 are regular season weeks. Weeks 18 through 21 are post-season weeks.

#### Input Parameters
* `format` - _required_ - Desired response format. Valid entries are <code>XML</code> or <code>JSON</code>.

## License

**flow**ground :- Telekom iPaaS / fantasydata-net-nfl-v-3-stats-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
