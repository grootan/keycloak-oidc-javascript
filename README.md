# Keycloak - Implicit Flow using Plain Javascript

This repo contains plain javascript example app that demonstrate the OpenId Connect's Implicit flow.

## Instructions

1. Clone / Download repository
2. Extract the zip or go to home directory
3. You can configure your OIDC related information in ```./index.html``` file
4. Make sure you replace `keycloak-tenant-id` with your TenantID and `keycloak-client-id` clientID from your keycloak.
5. Change `{hostname}` to match the domain of your keycloak
6. Need to install [http-server](https://www.npmjs.com/package/http-server), to serve the `index.html` file as localhost
7. RUN `npm i http-server -g` to install `http-server` as a global package
8. Once `http-server` is installed, RUN `http-server` in the same terminal, pointing to the root folder which has `index.html` file
9. You will receive a localhost URL, open that specific URL in the browser to view your initial screen

### Example

```sh
Starting up http-server -p <PORT_NUMBER>, serving ./
Available on:
  http://127.0.0.1:<PORT_NUMBER>
Hit CTRL-C to stop the server
```

## Approach to work with the implicit flow

1. Click on "login" button
2. You will be redirected to "Keycloak" user authentication screen
3. Complete all authentication steps
4. You will receive Token based on the response type which you configured

## What can I use these for

OpenId Connect is a great way to add user authentication to your application where you are depending on another party to manage the user identities.

In this case Keycloak will manage the identity of your users making it faster to get up and running.

## Single Sign On (SSO)

By implementing OpenId Connect via Keycloak you are creating a session which can be used to single sign on from your custom app into other apps that your users may have access to via the Keycloak portal

If you have any queries / you notice any issues don't hesitate to raise issue.
