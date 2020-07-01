<p align="center">
  <a href="https://www.gatsbyjs.org">
    <img alt="Gatsby" src="https://www.gatsbyjs.org/monogram.svg" width="60" />
  </a>
</p>
<h1 align="center">
  Gatsby's Starter: Uno
</h1>

Gatsby starter for creating a blog and showcasing your work with landing pages for earch portfolio item.

[Live Demo](https://22boxes-gatsby-uno.netlify.com/)

## Gatsby Recipe

This application had Auth0 added to it via a Gatsby Recipe. You can find that recipe [here](https://gist.github.com/twclark0/0e11c962743f4e62ccd33a92d8b52d23). You must use the "Raw" version of the gist.

## Auth0

Head on over to your [Auth0 Dashboard](https://manage.auth0.com). Do the following steps to set up an Auth0 application:

1. Click the "+ CREATE APPLICATION" button.
2. Name your new app (e.g. gatsby-recipe-auth0) and select "Single Page Web Applications". Hit "Create".
3. In the **Settings** for your new Auth0 application, add `http://localhost:8000` to the **Allowed Callback URLs**, **Allowed Logout URLs**, and **Allowed Web Origins**. Hit "Save Changes" at the bottom of the page.

Now that we have created our Auth0 application let's grab the values that we need. Under the **Settings** tab at the top, we will see our **Domain** and **Client ID**. 

Back in the code for our project, navigate to `src/gatsby-config.js`. Here we are going to scroll down find the following code block:

```javascript
{
  resolve: "gatsby-plugin-auth0",
  options: {
    domain: "yourdomain.auth0.com", // update this line
    clientId: "s0m3r4nd0mCh4raCT3rZ", // update this line
  },
},
```

The `domain` and `clientId` are values we will be updating. We will use our own Auth0 values and input that information here. 

## Deploy

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/iamtherealgd/gatsby-starter-22boxes-uno)

[![Deploy with ZEIT Now](https://zeit.co/button)](https://zeit.co/import/project?template=https://github.com/iamtherealgd/gatsby-starter-22boxes-uno)
