# Unraid Community Applications templates

This repository contains Unraid Community Applications templates maintained by Dennis Weyel.

## CalTopo History

CalTopo History is a self-hosted backup, versioning, recovery and audit application for CalTopo Team maps.

- Project: https://github.com/DWeyel/caltopo-history
- Container: `ghcr.io/dweyel/caltopo-history:latest`
- License: AGPL-3.0-only
- Persistent application data: `/data`
- Default Unraid appdata path: `/mnt/user/appdata/caltopo-history`
- Web UI container port: `8765/tcp`

On a fresh installation, CalTopo History generates a persistent application secret and a temporary initial `admin` password. The temporary password is printed to the container log on first start. Change it after signing in.

CalTopo service-account credentials can be configured from the application's Settings UI after installation. Plain HTTP works by default (`COOKIE_SECURE=false`); HTTPS with Secure session cookies is recommended for Internet-facing deployments.

## Community Applications submission

The repository follows the current Unraid Community Applications v2 template layout:

- `ca_profile.xml` — maintainer/repository profile
- `templates/caltopo-history.xml` — CalTopo History Docker application template
- `icon.svg` / `icon.png` — repository and application icons

After changes, validate and scan this repository through the Unraid Community Applications submission portal before submitting it for review.

## Support

For application questions and bug reports, use the CalTopo History GitHub repository:

https://github.com/DWeyel/caltopo-history/issues
