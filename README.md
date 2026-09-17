# Lotus

Lotus is a Linux-first VPN client with Xray, sing-box, WireGuard, and OpenVPN support.

## Downloads

Installable DEB and RPM packages, a portable Linux archive, SHA-256 checksums,
and GPG signatures are published on the
[Releases](https://github.com/ladyalcina/lotus/releases) page.

This repository is the public distribution channel for Lotus. The application core is maintained in a private repository; no user profiles, subscription links, credentials, diagnostics, or other private data are published here.

## Verify a download

The Lotus release-signing key has this fingerprint:

```text
6A62 B5D5 BCFD 7730 0335 5539 4682 7CF9 B946 8116
```

Download `lotus-release-signing-key.asc`, `SHA256SUMS`,
`SHA256SUMS.asc`, the package, and its matching `.asc` file from the same
release. Import the public key and verify its fingerprint:

```bash
gpg --import lotus-release-signing-key.asc
gpg --fingerprint 6A62B5D5BCFD77300335553946827CF9B9468116
```

Verify the signed checksum manifest before checking the package digest:

```bash
gpg --verify SHA256SUMS.asc SHA256SUMS
sha256sum --ignore-missing -c SHA256SUMS
```

The package itself can also be verified directly. For the Debian package, for
example:

```bash
gpg --verify lotus_0.35.1_amd64.deb.asc lotus_0.35.1_amd64.deb
```

The same public key is tracked in this repository at
[`keys/lotus-release-signing-key.asc`](keys/lotus-release-signing-key.asc).

## Supported platform

The maintained first release target is Linux. Android scaffolding exists but is not currently distributed.

## Issues

Use this repository for public installation and release issues. Never include VPN credentials, private keys, subscription URLs, or unredacted diagnostic logs in an issue.
