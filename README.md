# Keeper Draft Room

Keeper Draft Room is a private, read-only fantasy football analysis dashboard for two personal 12-team Yahoo leagues: one keeper league and one redraft league.

The project is designed to help one league manager understand roster construction, player availability, waiver options, trades, and matchups across both leagues. The keeper-league profile also supports keeper-cost and future-value analysis. It combines Yahoo league data with independently sourced fantasy rankings and projections to produce explainable recommendations tailored to each league's scoring and roster settings.

## Intended use

The application is limited to one user and two personal Yahoo Fantasy Football leagues. It is not a public or multi-user service. Yahoo Fantasy Sports API access will be used to retrieve:

- The authenticated user's leagues and teams
- League settings and scoring rules
- Team rosters
- Available players and waiver status
- Transactions
- Standings
- Weekly matchups

The application will cache responses locally and make a small number of requests during the football season.

## Read-only access

Keeper Draft Room requires read-only Yahoo Fantasy Sports API access. It will not:

- Add or drop players
- Submit waiver claims
- Set lineups
- Propose or accept trades
- Modify league settings
- Sell, redistribute, or publicly expose Yahoo data
- Provide Yahoo league data to other users

All roster moves and other league actions will continue to be completed by the user directly in Yahoo Fantasy Sports.

## Privacy and security

OAuth credentials and authorization tokens are stored outside the source repository. No Yahoo password is collected or stored. League data remains private and is used only for the authenticated user's personal analysis of the two leagues.

## Project status

The local Streamlit prototype is functional and has separate profiles for the keeper and redraft leagues. Yahoo Fantasy Sports API integration is the next planned feature and will replace manual roster and player-availability updates with authorized, read-only data retrieval for both profiles.

## Technology

- Python
- Streamlit
- Yahoo Fantasy Sports API
- OAuth 2.0

This is an independent personal project and is not affiliated with or endorsed by Yahoo.
