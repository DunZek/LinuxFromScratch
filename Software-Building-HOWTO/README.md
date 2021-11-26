# Building and Installing Software Packages for Linux
> Initialized: 2021-11-25. Last edited: 2021-11-25.

- v1.91, 27 July 1999
- Link: <https://tldp.org/HOWTO/Software-Building-HOWTO.html>

This is a comprehensive guide to building and installing "generic" UNIX software distributions under Linux. Additionally, there is some coverage of "rpm" and "deb" pre-packaged binaries.

## 1. Introduction
- Many packages for various UNIX and Linux flavors come as compressed archives of source files.
- Building the same package for different target machines allows the authr to save their self from having to produce multiple versions for various machines.
- The responsibility of installation however, then lies to the computer user.

## 2. Unpacking the Files
1. Download software package.
    - It's usually archived (*tarred*) and compressed (*gzipped*)..
    - ..in tarball form: `tar.gz` or `.tgz`
2. Copy to working directory.
3. *untar* and *gunzip* it:
    - `tar xzvf <filepath>`
    - De-archiving will 