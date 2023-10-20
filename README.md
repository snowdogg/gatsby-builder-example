<h1 align="center">
  Using Builder.io with Gatsby
</h1>

> A demo for integrating [Builder.io](https://www.builder.io) with Gatsby using our GraphQL API and the `@builder.io/gatsby` plugin

This demo demonstrates creating dynamic pages in Builder.io on new URLs and generating them with Gatsby, as well
as rendering specific parts of your site with Builder.io content via GraphQL queries (e.g. for pages, components, etc)

Run this example Gatsby project to see sample builder data, or replace the api key with your own to set up a Builder playground to learn how to integrate with Gatsby.

- [gatsby-config.js](gatsby-config.js) to set your API key

1.  **Sign up for Builder.io**
    Then replace the demo API key in gatsby-config.js with your public API key, which you can find in [builder.io/account/organization](https://builder.io/account/organization)

2.  **Clone this demo.**
  ``shell


  npm i
  npm run start
  ``

3.  **Connect Builder.io to your localhost**
  Now that you have the development server running on localhost, point the Builder.io entry to it by assigning the preview URL to be `http://localhost:3000`

When you deploy this to a live or staging environment, you can change the preview URL for your model globally from [builder.io/models](https://builder.io/models) (see more about models [here](https://builder.io/c/docs/guides/getting-started-with-models) and preview urls [here](https://builder.io/c/docs/guides/preview-url))

This example create pages dynamically based on the url you add to your entries on [Builder.io](https://www.builder.io), if you want to create a page manually, do not include the model in your `tempaltes` config as above, add a file under the `pages` folder and query all the entries your page needs from Builder.io, for example:
