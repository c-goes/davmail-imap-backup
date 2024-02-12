# Backup Exchange Account

Small (podman) compose  project with the purpose to backup the content of an Exchange mailbox by combining [davmail](https://davmail.sourceforge.net/) with [imap-backup](https://github.com/joeyates/imap-backup).


## How to use

````
mkdir backup-location  # where to backup the emails to
cp config.json.example config.json
# add username and password to the file
cp davmail.properties.example davmail.properties
# change the value for davmail.url in the file
chmod 0600 config.json
podman compose build
podman compose up
```