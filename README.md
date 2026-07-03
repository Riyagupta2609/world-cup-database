# ⚽ World Cup Database

A PostgreSQL database project that stores FIFA World Cup knockout stage match data from the 2014 and 2018 tournaments. The project includes automated data insertion using Bash scripting and SQL queries for data analysis.

## Features

- PostgreSQL relational database
- Automated data import from CSV using Bash
- Teams and games linked with foreign key relationships
- SQL queries for tournament statistics and analysis

## Technologies Used

- PostgreSQL
- Bash
- SQL

## Project Structure

```
.
├── worldcup.sql         # Database dump
├── insert_data.sh       # Imports data from games.csv
├── queries.sh           # SQL queries for analysis
├── games.csv            # Source dataset
└── README.md
```

## Database Schema

### Teams
- `team_id` (Primary Key)
- `name`

### Games
- `game_id` (Primary Key)
- `year`
- `round`
- `winner_id` (Foreign Key)
- `opponent_id` (Foreign Key)
- `winner_goals`
- `opponent_goals`

## Sample Queries

- Total goals scored
- Average goals per game
- Tournament champions
- Teams reaching knockout rounds
- Highest-scoring matches

## Learning Outcomes

- Designing relational databases
- Working with primary and foreign keys
- Importing CSV data using Bash
- Writing SQL queries with JOIN, GROUP BY, aggregate functions, and filtering

---

Built as part of the freeCodeCamp Relational Database Certification.
