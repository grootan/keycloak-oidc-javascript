# Keycloak - Implicit Flow using Javascript

This repository contains a JavaScript example application that demonstrates the implicit flow for OpenID Connect.

## Instructions

1. Clone / Download the repository
2. Extract the zip or navigate to the home directory.
3. You can customize the details relevant to the OIDC in the ```./index.html``` file.
4. Make sure that you replace the `keycloak-tenant-id` with your TenantID and `keycloak-client-id` clientID from your keycloak.
5. Modify `{hostname}` to align your keycloak domain.
6. Need to install [http-server](https://www.npmjs.com/package/http-server), to act as localhost to the `index.html`.
7. RUN `npm i http-server -g` as the global package to install `http-server`.
8. Upon installation of `http-server`, RUN `http-server` in the same terminal, referring/pointing to the root folder that has the `index.html` file.
9. You will receive a localhost URL, open that particular URL in your browser, to view your initial screen.

### Example

```sh
Starting up http-server -p <PORT_NUMBER>, serving ./
Available on:
  http://127.0.0.1:<PORT_NUMBER>
Hit CTRL-C to stop the server
```

## Approach to work with the implicit flow

1. Click on "login" button.
2. You will be redirected to the user authentication screen of "Keycloak".
3. Complete all of the authentication steps.
4. Depending on the response type you configured, you will receive a token.

## What can I use these for

OpenID Connect is a perfect way to incorporate user authentication to your application, where you are relying on another party to handle user identity.

In this situation, Keycloak handles the identity of the users, allowing it faster to get up and running.

## Single Sign On (SSO)

By integrating OpenID Connect via Keycloak, you are building a session that can be used to single sign-on from your custom app to other applications that your users can access via the Keycloak portal.

If you have any queries/you find any problems, please don't hesitate to raise an issue
