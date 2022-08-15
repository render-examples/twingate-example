# Twingate on Render
This repository demonstrates how to deploy the [Twingate Zero Trust solution](https://www.twingate.com) on the Render cloud. By using Twingate, you'll be able to directly access private resources that aren't exposed to the public web, such as [Render Private Services](https://render.com/docs/private-services) or [Render PostgreSQL](https://render.com/docs/databases) instances.

## Deployment

- _Log into_ your Twingate admin panel.
- _Create a network_ (**Network > Remote Networks** _(right sidebar)_ **> Add**) to continue. In the "type" dropdown select "Other" and name it `Render` (or whatever is meaningful to you).
- Click **Deploy Connector** in the right sidebar to..._deploy the connector_!
  - Select **Docker**, and _leave other settings as default_.
  - Click **Generate Tokens**, which will prompt you to re-authenticate your Twingate account.
  - You'll now have an `Access Token` and a `Refresh Token`. _Keep these handy_.

### One Click Deploy

Use the button below to deploy a Twingate connector on render.com. You will be asked to input your Twingate account URL (e.g. _https://acme.twingate.com_), access token and refresh tokens. You can obtain these values in your Twingate admin console

<a href="https://render.com/deploy?repo=https://github.com/render-examples/twingate/tree/main">
  <img src="https://render.com/images/deploy-to-render-button.svg" alt="Deploy to Render">
</a>
