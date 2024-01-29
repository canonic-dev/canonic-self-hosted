# Canonic Self Hosted

Deploy [Canonic](https://canonic.dev) on your own infrastructure. It's available as a simple docker image you can host anywhere.

## [Docs](https://canonic.dev/docs/self-hosted/getting-started)

This repository has a few examples that you can use to deploy Canonic to your favourite cloud provider.

## Docker Compose

Clone this repository, and navigate to it. Run the following command to start Canonic:

```bash
docker-compose up
```

You can now access the platform at `http://localhost:9191`

### Setting up SSL

If you have a domain on which you want to host your self hosted version, it is essential to set up SSL so that the domain can be accessed on https.

We have already configured nginx-proxy and acme-companion to provision the SSL certificate. In order to make it functional for your domain, make the following changes in the docker-compose file:

1. Change `VIRTUAL_HOST` and `LETSENCRYPT_HOST` to your domain where you want to host the app. For example `my-canonic.com`.

2. Change `DEFAULT_EMAIL` under nginx-proxy-acme environment to your email ID.

---

More coming soon!

Please provide all feedback at [support@canonic.dev](support@canonic.dev)
