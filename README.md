[ ![Download](https://api.bintray.com/packages/bincrafters/public-conan/lzma%3Abincrafters/images/download.svg?version=5.2.3%3Astable) ](https://bintray.com/bincrafters/public-conan/lzma%3Abincrafters/5.2.3%3Astable/link)
[![Build Status](https://travis-ci.org/SSE4/conan-lzma.svg?branch=testing%2F5.2.3)](https://travis-ci.org/SSE4/conan-lzma)
[![Build status](https://ci.appveyor.com/api/projects/status/liy7gce0098hdrm8/branch/testing/5.2.3?svg=true)](https://ci.appveyor.com/project/SSE4/conan-lzma/branch/testing/5.2.3)

XZ Utils is free general-purpose data compression software with a high compression ratio

[Conan.io](https://conan.io) package for [lzma](https://tukaani.org/xz/) project

The packages generated with this **conanfile** can be found in [Bintray](https://bintray.com/bincrafters/public-conan/lzma%3Abincrafters).

## For Users: Use this package

### Basic setup

    $ conan install lzma/5.2.3@bincrafters/stable

### Project setup

If you handle multiple dependencies in your project is better to add a *conanfile.txt*

    [requires]
    lzma/5.2.3@bincrafters/stable

    [generators]
    txt

Complete the installation of requirements for your project running:

    $ mkdir build && cd build && conan install ..

Note: It is recommended that you run conan install from a build directory and not the root of the project directory.  This is because conan generates *conanbuildinfo* files specific to a single build configuration which by default comes from an autodetected default profile located in ~/.conan/profiles/default .  If you pass different build configuration options to conan install, it will generate different *conanbuildinfo* files.  Thus, they should not be added to the root of the project, nor committed to git.

## For Packagers: Publish this Package

The example below shows the commands used to publish to bincrafters conan repository. To publish to your own conan respository (for example, after forking this git repository), you will need to change the commands below accordingly.

## Build and package

The following command both runs all the steps of the conan file, and publishes the package to the local system cache.  This includes downloading dependencies from "build_requires" and "requires" , and then running the build() method.

    $ conan create bincrafters/stable

## Add Remote

    $ conan remote add bincrafters "https://api.bintray.com/conan/bincrafters/public-conan"

## Upload

    $ conan upload lzma/5.2.3@bincrafters/stable --all -r bincrafters

### License
[LGPLv2.1/GPLv2/GPLv3](https://git.tukaani.org/?p=xz.git;a=blob;f=COPYING;hb=HEAD)