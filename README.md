<div align="center">

  [![AppMaker logo](https://avatars.githubusercontent.com/u/2833247?s=160)](#)<br>

  [![stable branch](https://img.shields.io/badge/dynamic/json.svg?logo=github&color=lightgrey&label=stable&query=%24.default_branch&url=https%3A%2F%2Fapi.github.com%2Frepos%2FUrsaDK%2FAppMaker)](https://github.com/UrsaDK/AppMaker)
  [![latest release](https://img.shields.io/badge/dynamic/json.svg?logo=github&color=blue&label=release&query=%24.name&url=https%3A%2F%2Fapi.github.com%2Frepos%2FUrsaDK%2FAppMaker%2Freleases%2Flatest)](https://github.com/UrsaDK/AppMaker/releases/latest)
  [![donate link](https://img.shields.io/badge/donate-coinbase-gold.svg?colorB=ff8e00&logo=bitcoin)](https://commerce.coinbase.com/checkout/c97803c0-459a-4994-b940-9ae197d176b8)

</div>

# AppMaker

This script is used to generate a new MacOS app which encapsulates either an executable file or a URL. If the app is generated around an executable, then the encapsulated file is run as soon as the app is opened. If a URL is given, then it is opened in a customised stand-alone Google Chrome window.

- [Requirements](#requirements)
- [Synopsis](#synopsis)
- [Changelog](#changelog)

## Requirements

  - [Google Chrome](https://www.google.com/chrome/) is required in order to encapsulate a URL.

## Synopsis

    appmaker [options] <url-or-file> <path-to-app>

    Create a MacOS app by encapsulating a given executable or URL into an app.
    The file will be copied inside the new app, and executed on app start.

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

        Arguments               All arguments are optional and
        ---------               can be supplied in any order.

        <url-or-file>           Path to the executable or the URL
                                to be encapsulated into the new app
        <path-to-app>           Path to the application

    <> - required parameters    [] - optional parameters
    Use 'less ./appmaker' to view further documentation.

## Changelog

 * 1.0.2

    - Bumped version number to get releases working on GitHub.
    - Updated documentation.

 * 1.0.1

   - Added default values to the output of `--help`.
   - Updated documentation

 * 1.0.0

   - Initial release of the code.
