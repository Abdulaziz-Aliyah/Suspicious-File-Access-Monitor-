# Suspicious-File-Access-Monitor

Python script that detects and alerts on repeated unauthorized access to sensitive files.

## Goal
A Python script that monitors an access log for repeated attempts to open sensitive files, and raises an alert when a user crosses a threshold.

## Tools
Python (file I/O, dictionaries)

## How it works
- Reads a log file (access_log.txt) line by line
- Flags any line mentioning a file in a watchlist (e.g. password.txt, secret.txt)
- Tracks how many times each user has accessed a sensitive file
- Prints an alert once a user's attempts reach 3 or more

## What I learned
How to parse log data programmatically, track per-user state with dictionaries, and design a simple rule-based detection system — a basic version of what a SIEM does at scale.

## Possible improvements
Add real timestamps, write alerts to a separate log file, support configurable thresholds. 