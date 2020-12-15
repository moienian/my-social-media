# my-social-media

This app is based on @hidjou tutorial on [freecodecamp Youtube channel](https://www.youtube.com/watch?v=n1mdAPFq2Os).


## Deployment

For deploy app, we use seprate host for client and server. For server, we use Heroku and for client, we use Netlify.

### Deploy backend to Heroku

Deployment app backend to Heroku is very easy. We can use Heroku CLI or linking Github repository with your Heroku account and leave all steps to himself!

Heroku give us an address for our app that we will using it for connet client to server.

### Deploy frontend to Netlify

Deploy app to Netlify is the similar way to Heroku. We can use Netlify CLI or deploy app by Github repository directly.

Before deploy client side of app to Netlify, we should make some change in client folder. First, we add `proxy` field to `package.json` file in client folder and assign server app address (already given us in previous step by Heroku) to it. Then we change entry uri in `createHttpLink` to same address in `/src/ApolloProvider.js` route.
