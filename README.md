# Sandbox Repository
Repository for various packages (used by spkg, a package manager.)
This is a special repo in that it supports *nix-In-A-Box apps, like LibTerm and OpenTerm.
The tool used to download packages from this repo will be similar to apt, using a Release file. See [here](https://github.com/sn3ksoftware/sandpkg).
This repo is still work in progress, so *use at your own risk.*

# - User-submitted software -

(You are strongly recommended to submit your software under a OSI-approved license, like the GPLv3.)

Users can submit a pull request with the command in this form:

For OpenTerm, tarball(tar -czvf) the whole .prideland command folder and submit a pull request, with a appropiate description in the metadata.plist file.

For Libterm (spkg is still wip), tarball(tar -czvf) the .py command by *itself* and submit a pull request. (Make sure its not nested in another folder!)

# •New repositories!!!•
The whole point of [spkg](https://github.com/sn3ksoftware/sandpkg) was to enable external repository support for pulling software.
Now you can, too! Create a RELEASE file in your repo in the Master branch under a "openterm" or a "libterm" folder, whichever platform you want to support. The RELEASE file is crucial as it contains a list of all programs in the repo.
(Particularly important because users will not know what programs they can install.
