Google Drive Backup
===================

A python script to sync your google drive contents.

:warning: This repository is not actively maintained. Some of the [forks](https://github.com/vikynandha/google-drive-backup/network) might be more up-to-date.

## Features
* You can Download your entire google drive or any given folder
* Downloads a file only if it has been modified since last download
* Logs all actions (optional)
* Uses OAuth2 authentication and can remember authentication

## Requirements
* Google API Python library. To install run
`pip install --upgrade google-api-python-client` or
`easy_install --upgrade google-api-python-client`

## Setup
* Edit `client_secrets_sample.json` and add your Google API client id and client secret (If you don't have one, [get it here](https://code.google.com/apis/console/)).
* Save it as `client_secrets.json`.
* Now, if you run `python drive.py [destination] [drive_id]`, a browser window/tab will open for you to authenticate the script. If you wish to download the entire Google Drive, use `root` in place of `[drive_id]`; otherwise, a folder id can be provided.
* Once authentication is done, the script will start downloading your *My Drive*. Refer the next section for more options.
