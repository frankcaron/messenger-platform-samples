# Stro TouchBistro Bot

This project is an adaptation of Facebook's sample Messenger chatbot for TouchBistro. We're using it to allow our customers and prospects to interact with TouchBistro's page.

Follow the [walk-through](https://developers.facebook.com/docs/messenger-platform/quickstart) to learn about this project in more detail.

## Setup

Ensure that the environment variables as follows are configured on your server:

## Run

You can start the server by running `npm start`. However, the webhook must be at a public URL that the Facebook servers can reach. Therefore, running the server locally on your machine will not work.

You can run this example on a cloud service provider like Heroku, Google Cloud Platform or AWS. Note that webhooks must have a valid SSL certificate, signed by a certificate authority. Read more about setting up SSL for a [Webhook](https://developers.facebook.com/docs/graph-api/webhooks#setup).

## Webhook

All webhook code is in `app.js`. It is routed to `/webhook`. This project handles callbacks for authentication, messages, delivery confirmation and postbacks. More details are available at the [reference docs](https://developers.facebook.com/docs/messenger-platform/webhook-reference).

## "Send to Messenger" and "Message Us" Plugin

An example of the "Send to Messenger" plugin and "Message Us" plugin are located at `index.html`. The "Send to Messenger" plugin can be used to trigger an authentication event. More details are available at the [reference docs](https://developers.facebook.com/docs/messenger-platform/plugin-reference).

## License

See the LICENSE file in the root directory of this source tree. Feel free to useand modify the code.