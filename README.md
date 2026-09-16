# Lotus

Lotus is a Linux-first VPN client with Xray, sing-box, WireGuard, and OpenVPN support.

## Downloads

Installable DEB and RPM packages, a portable Linux archive, SHA-256 checksums, and optional GPG signatures are published on the [Releases](https://github.com/ladyalcina/lotus/releases) page.

This repository is the public distribution channel for Lotus. The application core is maintained in a private repository; no user profiles, subscription links, credentials, diagnostics, or other private data are published here.

## Verify a download

Download the package together with `SHA256SUMS`, then run:

```bash
sha256sum -c SHA256SUMS
```

When detached signatures are available, verify them using the published Lotus release-signing public key.

## Supported platform

The maintained first release target is Linux. Android scaffolding exists but is not currently distributed.

## Issues

Use this repository for public installation and release issues. Never include VPN credentials, private keys, subscription URLs, or unredacted diagnostic logs in an issue.
