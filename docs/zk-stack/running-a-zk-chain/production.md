---
head:
  - - meta
    - name: "twitter:title"
      content: Deploying ZK Stack Chain to a Non-Local Environment | zkSync Docs
---

# Deploying to a Non-Local Environment

::: danger Note

A new and improved ZK Stack CLI is coming very soon. The current version is deprecated and may not function as expected.
:::

## Deploying to a non-local environment

The process to deploy to a non local environment is pretty similar to the local one. The wizard allows you to set up URLs to external services (database, RPCs, etc).

## Database

The wizard allows you to provide a custom database url connector. Make sure you provide it and that it accepts external connections if your server is not running in the same private network.

## Server (Sequencer) & Prover

After configuring your ZK Chain, you can generate docker images for your server and prover. To do that run `zk stack docker-setup`.

This command will guide you to properly name and tag your image. After building it, a docker compose file will be available so you can run the images on whichever cloud environment you desire.
