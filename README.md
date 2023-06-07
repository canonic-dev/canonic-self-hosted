# Canonic Self Hosted

Deploy [Canonic](https://canonic.dev) on your own infrastructure. It's available as a simple docker image you can host anywhere.

```bash
docker run -it \
  --platform=linux/amd64 \
  -p 3000:80 \
  -e "LICENSE=<YOUR_LICENSE_KEY>"
  trycanonic/canonic
```

## [Docs](https://canonic.dev/docs/self-hosted/getting-started)

This repository has a few examples that you can use to deploy Canonic to your favourite cloud provider.

## Docker Compose

Use the provided docker compose file to run Canonic with automatic updates enabled.

```bash
docker-compose up
```

---

Please provide all feedback at [support@canonic.dev](support@canonic.dev)
