# NFL Attendance Forecasting System

This project is an end-to-end data analytics and forecasting system focused on predicting NFL game attendance.
The initial scope includes a controlled subset of teams to support rapid development, validation, and scalability.

## Initial Scope (Module 1: Weeks 1–3)
- League: NFL
- Teams (8 total):
  - AFC West: Broncos, Chargers, Chiefs, Raiders
  - NFC South: Panthers, Buccaneers, Falcons, Saints

This scope includes representation from both conferences while keeping data volume manageable.

## Project Goals
- Build a scalable data pipeline for NFL game-level data
- Design a relational database to support forecasting models
- Enable expansion to additional divisions or the full league later in the semester
- Support future attendance forecasting using historical game and contextual data

## Data Sources
Primary data will be sourced from public NFL datasets available through the nflverse ecosystem and related Python-accessible sources.
Initial focus:
- Team metadata
- Game schedules and outcomes
- Game-level contextual variables

Play-by-play data is intentionally deferred due to size and is not required for early forecasting stages.

## Database Design (Initial)
- teams
- seasons
- games
- team_game_stats

The schema is designed so additional teams, seasons, and data sources can be added without redesign.

## Repository Structure
- data/raw/        Raw extracted datasets
- data/processed/ Cleaned datasets ready for modeling
- db/              SQLite database
- etl/             Extract, transform, and load scripts
- docs/            Project documentation and deliverables
