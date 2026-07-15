# Resources for ZED-Collab

# Introduction
These are some Notes to help People get started setting up ZED Collab Server using Podman.

**It doesn't currently work** since OIDC Login doesn't work (`zed-server` replies with 404 at `https://zed.MYDOMAIN.TLD/api/native_app_signin`).

The [ZED Collab Issue - Documentation](https://github.com/zed-industries/zed/issues/8260) of the ZED Collab Server describes the Issue.

This Repository contains just **ONE** possible implementation to help People get Started.

Contributions are welcome.

# Application Stack
- Reverse Proxy: Caddy
- Database: PostgreSQL
- OAuth Authentication: `oauth2-proxy` + Redis
- LiveKit + Redis
- Amazon S3-compatible Storage: Garage

`oauth2-proxy` is particularly interesting, since it can support both Human-to-Machine (Browser) and Machine-to-Machine (OAuth Token) Authentication.

# Server Setup
To be completed.

# Client Configuration
1. Open ZED IDE 
2. `Settings` -> `Network` -> `Server URL`: `https://zed.MYDOMAIN.TLD/api`
3. Restart the IDE
