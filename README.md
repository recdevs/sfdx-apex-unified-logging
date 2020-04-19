# Apex Unified Logging - SFDX Unlocked Namespaced Package

Logging framework based on Salesfore Platform Events to overcome the limitations of `System.debug` logging.

## Install: ##

- Installation URL: https://login.salesforce.com/packaging/installPackage.apexp?p0=04t5w000000iFisAAE
- Install from command line: `sfdx force:package:install -p 04t5w000000iFisAAE`

## Usage: ##

- Note 'My Domain' should be enabled in the org before using the log monitor
- Enable a trace:
  - Open Custom Settings setup page
  - select 'Settings' in aul namespace
  - select 'Manage' button
  - add a new Setting record (not org default)
  - enable for your user for the current date
- Open 'Sample App (Unified Logging)' (may need to be enabled in profile settings)
  - if the log monitor utility bar does not appear at the bottom of the screen then ensure 'My Domain' is enabled
- Open the log monitor from the utility bar at the bottom of the screen
- Execute `aul.Log.debug('test');`
- A log entry should appear in the monitor

## Features: ##
 - Provides unified view of logs over transaction boundaries (a.k.a. execution contexts)
 - Groups Logs of the same Batch
 - UI only shows the logs produced by current user
 - Autodetection of Code Location 
 - Nice UI using a Lightning Utility Bar 
 - Activated using user-level custom settings
 - Easily extendable to report exceptions and Governor Limit state
 
## Screenshots: ##

<img width="500" alt="lightning_experience___salesforce_und_skype_und_cprm____dev_projects_cprm__-_attributeprovider" src="https://user-images.githubusercontent.com/8180281/51395918-44efcf80-1b3e-11e9-978a-5e5ca4d29247.png">

<img width="500" alt="developer_console" src="https://user-images.githubusercontent.com/8180281/51323046-69c54380-1a67-11e9-9999-29d4697d4b82.png">

<img width="500" alt="custom_settings___salesforce" src="https://user-images.githubusercontent.com/8180281/51323040-6762e980-1a67-11e9-886a-159905a035db.png">

## Kudos to: ##

I was standing on the shoulders of those giants when building this

- [Advanced Logging with Platform Events](https://www.youtube.com/watch?v=yYeurYnasVc) by https://github.com/afawcett
- [Ein Versuch über einen Protokoll-Service](https://shoreforce.herokuapp.com/ein-versuch-uber-einen-protokoll-service/) by https://github.com/szandor72
- [Build an Instant Notification App](https://trailhead.salesforce.com/en/content/learn/projects/workshop-platform-events) 
