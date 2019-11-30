# Sandbox Repository
Repository for various packages (used by spkg, a package manager.)
This is a special repo in that it supports *nix-In-A-Box apps, like LibTerm and OpenTerm.
The tool used to download packages from this repo will be similar to apt, using a Release file. See [here](https://github.com/sn3ksoftware/sandpkg).
This repo is still work in progress, so *use at your own risk.*

# - User-submitted software -

(You are strongly recommended to submit your software under a OSI-approved license, like the GPLv3 or MIT License.)

Users can submit a pull request with the command in this form:

For OpenTerm, tarball(tar -czvf) the whole .prideland command folder and submit a pull request, with a appropiate description in the metadata.plist file.
Because spkg in OpenTerm relies on a RELEASE file, your package name should also be added there.

For Libterm (spkg is working somewhat), zip the .py command (stored in ~/Library/scripts) by *itself* and submit a pull request. (Make sure its not nested in another folder!)
~~If you had not installed zip yet, install with “package install zip”.~~ (The zip command from @ColdGrub1384’s repo is not working.
I will upload a (fairly) basic zip program here for Libterm soon, so run [spkg -i zip2] to install.)
spkg in Libterm is more advanced, and will automatically get the package list from the [Github REST API](https://api.github.com/repos/sn3ksoftware/sandboxrepo/contents/libterm)
so a RELEASE file is not needed. Just upload the package and everybody can download it right away.

# •New repositories!!!•
The whole point of [spkg](https://github.com/sn3ksoftware/sandpkg) was to enable external repository support for pulling software.
Now you can, too! Create a RELEASE file in your repo in the Master branch under a "openterm" or a "libterm" folder, whichever platform you want to support. The RELEASE file is crucial as it contains a list of all programs in the repo.
(Particularly important because users will not know what programs they can install.)

# Credits/Licenses
The credits for each script are stored in a plaintext contained in the same folder where that author’s package is.
Be careful to check the credits file first as this repository has more than one license for all its packages if you want to clone or fork the repo.
