## Data Descriptions

### daily_standings.csv
Contains the standings from every day a game was played going back to 2009-10 season.

#### Columns
- season
- date
- teamId
- conferenceName
- divisionName
- gamesPlayed
- goalAgainst
- goalFor
- homeGamesPlayed
- homeGoalsAgainst
- homeGoalsFor
- homeRegulationWins
- homeWins
- homeLosses
- homeOtLosses
- homePoints
- roadGamesPlayed
- roadGoalsAgainst
- roadGoalsFor
- roadRegulationWins
- roadWins
- roadLosses
- roadOtLosses
- roadPoints

### trade_dates.csv
Trade id and the date of the trade.

#### Columns
- tradeId
- trade_date

### traded_contracts.csv
Contract details for players involved in trades. `season` is the season end year for the season the contract was activate. `seasonStart` is the season a contract was first active. `seasonEnd` is the season a contract ends (expires at the conclusion). `aav` is the average annual value of the contract in dollars over the duration of the contract. `amountOfCapRetained` amount of the cap hit retained by `toTeamId` when `fromTeamId` receives the asset. `acquiringCap` is the effective aav of the contract for the receiving team (cap hit - cap retained)

#### Columns
- contractId
- playerId
- season
- seasonStart
- seasonEnd
- aav
- tradeId
- toTeamId
- fromTeamId
- amountOfCapRetained
- acquiringCap

### traded_draftpicks.csv
Details of draft picks involved in trades. `conditions` are the trade conditions placed on the draft pick, if any. `draftYear` is the year the draft pick is for. `round` is the round the draft pick is in. `overall` is the overall pick number of the pick, for future picks this is not filled in as that would not have been known at the time the trade was made.

#### Columns
- tradeId
- toTeamId
- fromTeamId
- conditions
- draftYear
- round
- overall

### traded_goalie_career.csv
Goalie stats leading up to the traded season. Regular season and post season stats are separated.

#### Columns
- playerId
- position
- positionGeneral
- league
- leagueLevel
- tradeId
- regularGoalsAgainst
- regularShotsAgainst
- regularShutouts
- regularSaves
- regularWins
- regularLosses
- regularOtLosses
- postseasonGoalsAgainst
- postseasonShotsAgainst
- postseasonSaves
- postseasonShutouts
- postseasonWins
- postseasonLosses
- postseasonOtLosses

### traded_goalie_platform.csv
Goalie stats for the most recent season before the trade. Regular season and post season stats are separated.

#### Columns
- playerId
- position
- positionGeneral
- league
- leagueLevel
- tradeId
- regularGoalsAgainst
- regularShotsAgainst
- regularShutouts
- regularSaves
- regularWins
- regularLosses
- regularOtLosses
- postseasonGoalsAgainst
- postseasonShotsAgainst
- postseasonSaves
- postseasonShutouts
- postseasonWins
- postseasonLosses
- postseasonOtLosses

### traded_player_general_info.csv
General biographical information of the players.

#### Columns
- playerId
- position
- positionGeneral
- height_cm
- weight_kg
- handedness
- dateOfBirth
- birthCountry
- draftYear
- draftRound
- draftOverallPick

### traded_skater_career.csv
Skater stats leading up to the traded season. Regular season and post season stats are separated. `atoi` is the average ice time for the skater per game in seconds. `pp_atoi` is the average ice time during the power play per game in seconds. `pk_atoi` is the average ice time during the power play per game in seconds

#### Columns
- playerId
- position
- positionGeneral
- league
- leagueLevel
- tradeId
- regularGamesPlayed
- regularGoals
- regularAssists
- regularPenaltyMinutes
- postseasonGamesPlayed
- postseasonGoals
- postseasonAssists
- postseasonPenaltyMinutes
- regular_hits
- regular_blockedShots
- regular_powerplayGoals
- regular_shots
- regular_atoi
- regular_pp_atoi
- regular_pk_atoi

### traded_skater_platform.csv
Skater stats leading up to the traded season. Regular season and post season stats are separated.

#### Columns
- playerId
- position
- positionGeneral
- league
- leagueLevel
- tradeId
- regularGamesPlayed
- regularGoals
- regularAssists
- regularPenaltyMinutes
- postseasonGamesPlayed
- postseasonGoals
- postseasonAssists
- postseasonPenaltyMinutes
- regular_hits
- regular_blockedShots
- regular_powerplayGoals
- regular_shots
- regular_atoi
- regular_pp_atoi
- regular_pk_atoi

