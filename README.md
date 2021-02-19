# home-server

Home gateway server that has some ports open to the public internet. SSH,
Fail2Ban, WireGuard.

## WARNING

**Only install public keys from devices with encrypted drives and trusted boot
such as Android, iPhone, Chrome.**

## Motiviations

1. Secure SSH from any device (ssh with password + TOTP)
1. Easy SSH from trusted devices (ssh with public key, but only from devices
   with encrypted drives and secure boot, so Android and Chrome.)
1. Discourage script kiddies - using Fail2Ban.
1. Full VPN access from trusted devices

## Extra install steps

* Don't forget to run `public/bin/setup-totp-file.sh` for each user that wants
  ssh access. This sets up TOTP (2FA codes) - so have a client ready to scan the
  ASCII QR code.

