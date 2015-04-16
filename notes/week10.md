% Week 10
% Network Authentication & Git
% April 9 2015

# Authentication

## Passwords for VCS?

Why would we need to put access control on a repository?

> * Private
> * Limited Permissions (read or write)
> * Vandalism

## How does git handle authentication?

*Git doesn't*

. . .

It defers to the transport.

## Review transports

* file
* http
* **ssh**

## Lets get to the meat and potatoes

# SSH Authentication

## But this only paves the road...

The client must prove who it says it is.

* password
* kerberos
* **public key**

## Public Key Cryptography

Is a asymmetric cryptographic process which produces **two** keys.

* Private key
    * Encrypt
    * Decrypt
* Public key
    * Encrypt

## Proof of identity

Given it knows you public key you claim to have, a SSH server can **enncrypt** a
256 bit random string. 

. . .

Your client uses the private key to decrypt this string proving you have the
private portion of the asymmetric key pair. Boom, you have authenticated.

# Let's do this!

## Environment

I am going to use windows.

. . .

* The offical git binary
    * git-scm.com/downloads
* Sublime Text

## Key Generation

The ssh client software suite includes several programs, including ssh-keygen.
This program creates the two component keys with given parameters.

. . .

The passphrase is a password that wraps a key. You should have one, but you
don't have to.

## Add key to Github User

Most interfaces have a section in their user settings that lets you manage your
public keys.

## Lets try!

We can clone the course content repo!

## Password Management

Having the puss phrase prevents someone from easily impersonating you. But you
don't want to type the passphrase everytime.

. . . 

Introduce the ssh-agent

## ssh-agent
A small program that keeps keys in memory and renders them on request. It is not
started by default, but can be!


# Questions & Hands On
