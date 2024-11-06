# Lavalink v4 Pterodactyl Egg

This repository contains a Pterodactyl egg for deploying a high-performance Lavalink v4 audio server within the Pterodactyl panel, tailored for optimal audio streaming for applications like Discord bots.

## Features
- **Docker Image**: Uses `ghcr.io/coho04/pterodactyl-docker-images:java_21`, a Java 21 environment tailored for Lavalink.
- **Dynamic Configuration**: Automatically configures `application.yml` with the server’s assigned port.
- **Automated Installation**: Fetches the latest Lavalink `.jar` and configures necessary files during installation.

## Installation
1. Import this egg into your Pterodactyl panel.
2. Create a new server using the Lavalink egg.
3. Start the server, and the installation script will handle the rest, including downloading and configuring Lavalink.

## Important
To change the password, you’ll need to edit the `application.yml` file after installation. Locate the `server` section within the file and update the `password` field to your desired password for secure access.

## Usage
The Lavalink server will start automatically on the assigned port, which is dynamically set by Pterodactyl for seamless integration.

**Note**: Avoid manual edits to the `application.yml` port configuration, as it’s automatically set by Pterodactyl to match the server’s assigned port.
