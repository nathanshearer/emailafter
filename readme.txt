Description:
  Send an email after running a command.

Usage:
  emailafter [options] mail@example.com command [args]

Options:
  -h, --help
    Display this help message and exit.
  -p, --pretend
    Print out the e-mail address and the command that would be executed.

Examples:
  emailafter -p mail@example.com du --apparent-size -b -l -x /mnt/storage
  emailafter mail@example.com cp -afv /mnt/storage /mnt/backup
  emailafter mail@example.com 7z a /mnt/offsite/storage.7z /mnt/backup/storage

Version:
  emailafter 1.1.0.0
  Copyright (C) 2018 Nathan Shearer
  Licensed under GNU General Public License 2.0
