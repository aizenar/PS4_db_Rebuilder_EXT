# PS4_db_Rebuilder_EXT

Ps4 built-in database rebuilder has the tendency to remove fpkg from the database. This will repopulate the database with them!

This repository is a modification of the Zer0xFF repository (https://github.com/Zer0xFF/PS4_db_rebuilder) but with the improvement that it now processes all games and homebrews (RetroArch, Ps4-Xplorer, PS2 games, ...).

## Requirement

- Python (preferably 3.0+)

## Instructions

1) Recursively clone (`git clone <url> --recursive`)  this repo or download a release (https://github.com/aizenar/PS4_db_Rebuilder_EXT/releases/download/v0.1/PS4_db_Rebuilder_EXT-0.1.zip)
2) Start FTP server on the PS4
3) Run the python script through terminal/cmdline:
	
	| Version | Command |
	|--|--|
	| 5.05 | `python3 fix_db.py [PS4_IP] --port [PS4_FTP_PORT] --fw 5.05` |
	| 6.72 - 7.02 | `python3 fix_db.py [PS4_IP] --port [PS4_FTP_PORT]` |

4) Wait for the script to finish, then logout of the PS4 user without closing the browser

5) Log back in and all your games should be there again

## Changes

1) Original Repo https://github.com/Zer0xFF/PS4_db_rebuilder
2) Update fix_db.py so now it also processes homebrew applications and other installed packages (PS2 games, ...)
3) Update fix_db.py so now you can use a custom FTP port

