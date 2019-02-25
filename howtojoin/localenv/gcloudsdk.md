# Install and setup Google Cloud SDK

## Install Google Cloud SDK

Download and execute installer to your pc.

Google Cloud SDK:  
https://cloud.google.com/sdk/

After install, check 'gcloud' command is enable.

```
$ gcloud version
Google Cloud SDK 193.0.0
```

## Install Component

Install 'gcloud app Java Extensions'.

```
gcloud components install app-engine-java
```

setup 'APPENGINE_HOME' environment variable.

```
export APPENGINE_HOME=<<put your google-cloud-sdk path>>/platform/google_appengine/google/appengine/tools/java/
```

## Check Run App Engine Local Development Server

clone Repository of Service.

```
git clone git@github.com:<organization>/<repository>.git
```

Start App Engine Local Development Server.

```
cd <repository>
gradle appengineRun
```

access to following url  by your web browser.
- http://localhost:8080/actuator/health ... health check response
- http://localhost:8080/_ah/admin ... development console
