## Pantheon site updates
Bash shell script to check core and contrib module/plugin updates for all available Pantheon sites

- Works for Drupal 7, Drupal 8 and WordPress sites hosted on Pantheon
- Supports Drush 9

## Prerequisites:
- [Terminus](https://github.com/pantheon-systems/terminus)
- [Terminus Composer Plugin](https://github.com/pantheon-systems/terminus-composer-plugin) -
 _Only needed for Composer managed Drupal 8 sites using Drush 9_

## Install:
```
$ git clone git@github.com:uberhacker/pantheon-site-updates.git
$ sudo cp pantheon-site-updates/checkupdates /usr/local/bin/
```
## Usage:
### Check updates on all sites (errors to stdout)
```
$ checkupdates > report.txt
```
### Check updates on all sites (ignore errors)
```
$ checkupdates > report.txt 2> /dev/null
```
### Only report errors to file
```
$ checkupdates 2> error_report.txt
```
### Check updates and report errors to file
```
$ checkupdates &> full_report.txt
```
