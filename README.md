# Cloud Foundry Django sample app: Tasks

This is a basic Python Django app designed to run on a cloud foundry python buildpack.
It allows the user to store tasks and display all tasks. Requires a postgresql service.
*It is not an example of good django project structure or best practices* but to test the platform.

## Prerequisite

You need PostgreSQL as a backing service. activate it with

```cf create-service postgresql v9.4-dev postgres-service```

## Deploying the app

Also you have to adjust the name of your app to be unique. Edit **manifest.yml** to do that. Use i.e. your username you find behind the user icon in the SCP cockpit.

Then change to the folder to which you've cloned the app and you can push it with

```bash
cf push
```
