Description:
  Run a command then send the command, statistics, and output in an e-mail.

Usage:
  emailafter [options] command [args]

Options:
  -c, --config emailafter.conf
    Load emailafter.conf after trying /etc/emailafter.conf and ~/.emailafter.conf
  -e, --email mail@example.com
    Send the e-mail to mail@example.com
  -h, --help
    Display this help message and exit.
  -n, --lines 100
    Send up to the first and last 100 lines of the command output.
  -p, --pretend
    Print out the e-mail address and the command that would be executed.

Examples:
  emailafter -p -e mail@example.com du --apparent-size -b -l -x /mnt/storage
  emailafter -e mail@example.com cp -afv /mnt/storage /mnt/backup
  emailafter -e mail@example.com 7z a /mnt/offsite/storage.7z /mnt/backup/storage

Version:
  emailafter 2.0.0.0
  Copyright (C) 2018 Nathan Shearer
  Licensed under GNU General Public License 2.0
