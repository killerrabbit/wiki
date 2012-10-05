---
title: Installation &raquo; Mac OS X
layout: default
---

InspIRCd packages are available in the [Homebrew package manager](http://mxcl.github.com/homebrew/).

## Installation

First, ensure that your copy of Homebrew is up to date by executing the following command:

    brew update

Now that your copy of Homebrew is up to date, you can install the InspIRCd package using the
following command:

    brew install inspircd

InspIRCd will now be downloaded and installed from source. Once it has finished installing, it will
be available as a keg-only package in your Homebrew directory. This will usually be located at
`/usr/local/Cellar/inspircd/X.Y.Z/`.

## Extra Modules

Extra modules can be enabled at install time by passing an option to the install command. A list of
possible options can be found by using the following command:

    brew info inspircd

## Related Links

* [Homebrew &mdash; The missing package manager for OS X](http://mxcl.github.com/homebrew/)
