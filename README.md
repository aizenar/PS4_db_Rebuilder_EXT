# PS4_db_rebuilder

Ps4 built-in database rebuilder has the tendency to remove fpkg from the database. This will repopulate the database with them!

## Requirement

- Python (preferably 3.0+)

## Instructions

1) Recursively clone (`git clone <url> --recursive`)  this repo or downdload a release.
2) Start FTP server on the PS4
3) Run the python script through terminal/cmdline:

	**For 5.05:
	python3 fix_db.py [PS4_IP] --port [PS4_FTP_PORT] --fw 5.05 
	
	**For 6.72 to 7.02:
	python3 fix_db.py [PS4_IP] --port [PS4_FTP_PORT]

4) Wait for the script to finish, then logout of the PS4 user without closing the browser

5) Log back in and all your games should be there again

## Changes

1) Original Repo https://github.com/Zer0xFF/PS4_db_rebuilder
2) Update fix_db.py so now it also processes homebrew applications and other installed packages (PS2 games, ...)
3) Update fix_db.py so now you can use a custom FTP port

