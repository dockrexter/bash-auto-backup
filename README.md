# Bash Auto Backup

A lightweight Bash script that automates daily file backups by creating timestamped archives of recently modified files.

## Features

- Backs up files modified in the last 24 hours
- Creates timestamped `.tar.gz` archives
- Supports cron scheduling for automation
- Simple validation and error handling

## Installation

Clone and setup:

git clone https://github.com/yourusername/bash-auto-backup.git
cd bash-auto-backup
chmod +x backup.sh

## Usage

Manual backup:

./backup.sh <source_directory> <destination_directory>

Example:

./backup.sh /home/user/documents /home/user/backups

## Cron Automation

Edit crontab:

crontab -e

Daily backup at 2:00 AM:

0 2 * * * /path/to/backup.sh /home/user/documents /home/user/backups

## License

MIT License
