# Dock
**Deploying docker containers is as easy as 'git push'**

Dock is a bash script that tracks changes to a git repository, and when new code is pushed, rebuilds and runs the the changes. Dock also comes with some other handy features, such as restarting containers that have stopped, and cleaning up docker artifacts to save disk space.

### Installation
The easiest way to install dock is to create a cron job. To set dock to check hourly for changes run the following:

``` bash
$ crontab -e
00 * * * * /path/to/dock /path/to/git/repo
```
