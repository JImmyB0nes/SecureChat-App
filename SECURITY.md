# Security policy

Enigma 3 is end-to-end encrypted. What that means in practice, and where the
limits lie, is documented in the app itself and in the release notes.

## Report an issue

Please open a [**GitHub issue**](https://github.com/JImmyB0nes/SecureChat-App/issues)
for anything you consider a security problem. There is no separate reporting
channel — if you are unsure whether something is a vulnerability, open an issue
and it will be triaged.

We confirm receipt within 72 hours and deliver an assessment within 14 days.

## What we consider a vulnerability

- Anything that bypasses or weakens the end-to-end encryption.
- Key access through the app (vault, keystore, DPAPI, PIN handling).
- The update path: signature verification, checksums, the manifest.
- Device binding that can be silently undermined.
- Remotely exploitable flaws in the web view or the Capacitor layer.

## What we do not consider a vulnerability

- Attacks that already require physical access to your unlocked device.
- Copies on recipient devices (screenshots, downloads).
- Antivirus warnings about the unsigned installer.
- Dependencies that only matter on an already compromised machine.

When in doubt: report it once more rather than once too little.

## Updates

Updates run through the desktop app or this repository. The app checks every
version against a built-in Ed25519 signature and the SHA-256 checksum of the
file. Both are published in the release.
