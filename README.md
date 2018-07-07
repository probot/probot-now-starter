# {{ name }}

> a GitHub App built with [probot](https://github.com/probot/probot) that {{ description }}

## Setup

After you [Create a GitHub App](https://probot.github.io/docs/deployment/#create-the-github-app), use the [Now CLI](https://github.com/zeit/now-cli) to add your app's environment variables using the [`now secrets`](https://zeit.co/docs/getting-started/secrets) command:

```sh
# Add environment variables to Now
now secrets add app-id <your-app-id>
now secrets add webhook-secret <random-webhook-secret>

# Download your private key to the root of this project and use base64 encoding to add it to Now
now secrets add private-key-base64 '$(cat ./private-key.pem | base 64)'

# Install dependencies
npm install

# Run the app locally
npm start

# Deploy to now
now
```

See our docs for more information on [deployment to Now](https://probot.github.io/docs/deployment/#now)
