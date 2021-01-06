# Sample Hello World Python app for OCP
Quick hello world app that uses express.js - sample created as quick import for OCP
This application is compiled against GUNICORN and WSGI web server, this is not to be used in production this way.

## To run this application
```
1. oc new-project <project name>
2. oc new-app nodejs~https://github.com/quivsoth/redhat-nodejs-helloworld
3. oc expose svc/redhat-nodejs-helloworld
4. From the topology window click on the newly created pod and look for the newly created route
5. Optional: Label the icon with "oc label dc app.kubernetes.io/name=python"
```
