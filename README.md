# easypki-ovpn
Make it easy to manage an OpenVPN PKI

## Dependencies
Make sure you have a working copy of [easypki](https://github.com/google/easypki) in your path.
For Alpine Linux based installs you can simply install it by: `apk add easypki`.

## Setup
Create a config directory by copying it from the provided sample directory:
`cp -r sample config` and edit the files to update the settings.

## Operation
Simply run the script found in the root of the release `easypki-ovpn` for help.

```txt
easypki-ovpn:

    easypki-ovpn will make it easy to setup a PKI certificate authority
    Diffie-Hellman parameters static TLS key and generate OpenVPN inline (ovpn)
    user configuration files.

Usage: ./easypki-ovpn command

Available commands:
    init:       Initialize new pki store including server certificate and keys
    create:     Create new user
    list:       List users

Available options:
    create:
        -u user common name
        -e user email address
    general:
        -h This help
```
