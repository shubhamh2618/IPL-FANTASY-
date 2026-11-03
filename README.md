# L19 – IPL Fantasy Points

**Student:** HINGRAJIYA SHUBHAM SANJAYBHAI | **Roll:** D18 | **Division:** H | **Enrollment:** 24004501210107

## Problem
Create a fantasy points calculator that scores players from match stats and picks the best XI.

## Who will use it
A friends' IPL fantasy league.

## Folder structure
- main.sh – menu (run with ./main.sh)
- lib/functions.sh – all functions
- data/ – data files
- reports/ – reports created by the script
- backups/ – tar.gz backups
- logs/ – activity.log and cron.log

## Features
1. Calculate fantasy points with a formula in awk
2. Top 11 players overall
3. Team-wise total points
4. Best player per role
5. Points report file

## How to run
    cd ~/linux_project/fantasyxi
    ./main.sh
    ./main.sh --help

## Crontab task
Every day at 11 PM during the league, recalculate fantasy points and rankings

    0 23 * * * /bin/bash $HOME/linux_project/fantasyxi/main.sh --cron >> $HOME/linux_project/fantasyxi/logs/cron.log 2>&1

## Commands used
awk, sort, head, grep, printf

## What I learned
## What I learned
- Learned to write menu-driven shell scripts using Bash.
- Used awk to calculate fantasy points from CSV data.
- Practiced sorting and filtering player records.
- Learned file handling, logging and backup using tar.gz.
- Learned to schedule automated tasks using Cron.
