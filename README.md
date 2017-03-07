# flask_appengine_redirector
Google App Engine Flask C2 redirector 

A simple Python Flask example application that's ready to run on App Engine.

## Development Setup

* Install SDK: https://cloud.google.com/sdk/docs/

* Run dev instance: `dev_appserver.py app.yaml`

## Deploy

* `gcloud app create`

* `gcloud app deploy`

## Setup 
set debug output to the log outlet (Defaults to True:
set forward C2 domain (Where to redirect to):
set redirector domain (Incoming domain name):
```
env_variables:
DEBUG: True
FORWARD_DOMAIN: 'cybersyndicates.com'
CURRENT_DOMAIN: 'mineral-highway-136423.appspot.com'
  ```

## Monitor 
monitor the dyno:
* `gcloud app logs tail`