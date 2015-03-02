# CRONTRAIN (only works on OS X)

## Installation:

```
./install.sh
```


## Configure crontab

1. Edit the crontab to your liking
2. Add the crontab rules to your crontab

### Little help

To be safe, backup your current crontab in a file:
```
crontab -l > crontab.backup
```

then put back the current crontab and the new one to your crontab:

```
cat crontab crontab.backup > crontab.tmp
crontab > crontab.tmp
rm crontab.tmp
```

If the cronjob fails for some reasons, ```cron``` takes care of sending an email (type: ```mail``` in a terminal to read them).
