AppMaker
========

**Version:** 1.0.1
**Status:** Fully functional, but missing tests.

This script is used to generate a new MacOS app which encapsulates either an executable file or a URL. If the app is generated around an executable, then the encapsulated file is run as soon as the app is opened. If a URL is given, then it is opened in a customised stand-alone Google Chrome window.

Requirements
------------

- [Google Chrome](https://www.google.com/chrome/) is required in order to encapsulate a URL.

Synopsis
--------

    appmaker [options] <url-or-file> <path-to-app>

    Create a MacOS app by encapsulating a given executable or URL into an app.
    The file will be copyed inside the new app, and executed on app start.

        Options                 All options are optional and
        -------                 can be supplied in any order.

        -c --copyright=<str>    Copyright for the new application
        -f --force              Overwrite existing app (use with care)
        -i --icon=<path>        A path to the app icon (must be a square)
                                Supported formats: ICNS, PNG, GIF, JPG
        -n --appname=<str>      App name, as it appears in the menu
                                Lenght: 16 characters maximum
        -v --appversion=<x.x.x> Application version number

        -l --log=<path>         Redirect all output to a file
        -q --quiet              Suppress output of the script
        -? --help               Display this help message
        --version               Script and BASH version info

        Arguments               All agruments are optional and
        ---------               can be supplied in any order.

        <url-or-file>           Path to the binarry or the URL which is
                                to be encapsulated into the new app
        <path-to-app>           Path to the application

    <> - required parameters    [] - optional parameters
    Use 'less ./appmaker' to view further documentation.

Changelog
---------

* 1.0.0

  - Initial release of the code.

Donations
---------

This script is 100% free and is distributed under the terms of the MIT license. You're welcome to use it for private or commercial projects and to generally do whatever you want with it.

If you found this script useful, would like to support its further development, or you are just feeling generous, then your contribution will be greatly appreciated!

<p align="center">
  <a href="https://paypal.me/UmkaDK"><img src="https://img.shields.io/badge/paypal-me-blue.svg?colorB=0070ba&logo=paypal" alt="PayPal.Me"></a>
  &nbsp;
  <a href="https://commerce.coinbase.com/checkout/c97803c0-459a-4994-b940-9ae197d176b8"><img src="https://img.shields.io/badge/coinbase-donate-gold.svg?colorB=ff8e00&logo=bitcoin" alt="Donate via Coinbase"></a>
</p>
