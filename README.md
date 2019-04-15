# Sandbox Repository
Repository for various Python Index Packages and sandman (Sandboxed Package Manager).
This is a special repo in that it supports *nix-In-A-Box apps, like LibTerm and OpenTerm.
The tool used to download packages from this repo will be similar to apt, using a Release file.
This repo is still work in progress, so *use at your own risk.*

(The sandman CLI code itself is under the GPLv3 license for all purposes.)

## Why sandman?
I wanted to try to integrate pip into Libterm by running the default install script,
but it does not work by itself. So, I started this repo to host packages that I modified to work in Libterm.
The main inspiration of sandman was [StaSh](https://github.com/ywangd/stash).

# - Installation (WIP, not ready yet) -

## OpenTerm
Run these commands in your shell.

```
curl -O https://github.com/sn3ksoftware/sandboxrepo/raw/master/openterm/install.cub

cub install.cub
```

## Libterm
Run this command:

```
curl -O https://github.com/sn3ksoftware/sandboxrepo/raw/master/libterm/install.sh && sh install.sh
```

# - User-submitted software -
I know that Libterm already has something like this, but before you accuse me of reinventing the wheel let me explain.
OpenTerm did not have a package manager, so I created one.
But for Libterm, there was no external repo support for its inbuilt file manager.
Thus, I created sandman to make it easier to test and pull software.

Users can submit a pull request with the command in this form:

For OpenTerm, gzip the whole .prideland command folder and submit a pull request, with a appropiate description in the metadata.plist file.

For Libterm, just zip the .py command by *itself* and submit a pull request. (Make sure its not nested in another folder!)

# •New repositories!!!•
The whole point of sandman was to enable external repository support for pulling software.
Now you can, too! Create a RELEASE file in your repo under a "openterm" or a "libterm" folder, whichever platform you want to support. The RELEASE file is crucial as it contains a list of all programs in the repo.

# - FAQ -
Q: I thot that Libterm has a package manager already?

A: Read the point under user-submitted software.

Q: Will I get credited for any software I upload to this repo?

A: Defintely! You also should put credits in your code as a good habit.

Q: Who is sandman for?

A: CLI masters and programmers who have at least basic command-line skills.
