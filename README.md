# Locker

A tool for provisioning PHP projects using Docker and Docker Compose. Locker can manage all of your dev, stage, and production deployments.

## Requirements

- Docker
- Docker Compose
- A Docker host such as:
  - Virtualbox and Boot2Docker (for local development)
  - A Docker Machine host (for staging and production environments)

## Install

The easiest way is to include Locker in your `composer.json` file.

    "require": {
        "ricog/locker": "0.1.*",
	}

## Configure

Locker needs a `locker.yml` file to run. The best place for this is in your root folder, or in a `locker` folder at the root of your project. In fact, Locker will look in both locations. Use the `locker-sample.yml` file as a starting point.

## Use

To get a full list of commands and options.

	bin/locker

Start your containers.

	bin/locker up
