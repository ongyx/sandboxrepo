# Sandbox Repository
Repository for various packages (used by spkg, a package manager.)
This is a special repo in that it supports *nix-In-A-Box apps, like LibTerm and OpenTerm.
The tool used to download packages from this repo will be similar to apt, using a Release file. See [here](https://github.com/sn3ksoftware/sandpkg).
This repo is still work in progress, so *use at your own risk.*

# - User-submitted software -

Users can submit a pull request with the command in this form:

For OpenTerm, gzip the whole .prideland command folder and submit a pull request, with a appropiate description in the metadata.plist file.

For Libterm, just zip the .py command by *itself* and submit a pull request. (Make sure its not nested in another folder!)

# •New repositories!!!•
The whole point of sandman was to enable external repository support for pulling software.
Now you can, too! Create a RELEASE file in your repo under a "openterm" or a "libterm" folder, whichever platform you want to support. The RELEASE file is crucial as it contains a list of all programs in the repo.
