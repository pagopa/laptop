PagoPA Developer Laptop
======
PagoPA Developer Laptop is a script to set up a macOS computer for development, and to keep
it up to date. It's forked from the [original](https://github.com/thoughtbot/laptop).

It's very opinionated to our company needs in terms of stack and culture.

It can be run multiple times on the same machine safely. It installs,
upgrades, or skips packages based on what is already installed on the machine.


Requirements
------------

Supported operating systems:

* macOS Catalina (10.15)
* macOS Mojave (10.14)
* macOS High Sierra (10.13)
* macOS Sierra (10.12)
* OS X El Capitan (10.11)
* OS X Yosemite (10.10)
* OS X Mavericks (10.9)

Older versions may work but aren't regularly tested. Bug reports for older
versions are welcome.

NOTE: For updates, we assume that ZSH_CUSTOM folder is at $ZSH/custom

What it does
-------

* Configure OSX command line tools, if not present
* Install and configure Homebrew, if not present
* Install several applications via Homebrew, including `Visual Studio Code` (Please see `Brefile` for details)
* Configure Visual Studio Code by installing plugins and setting up `code` command if not present
* Create basic Visual Studio Code user settings, if not present
* Install [oh-my-sh](https://github.com/ohmyzsh/ohmyzsh) and [spaceship](https://github.com/denysdovhan/spaceship-prompt) theme.

How to use
-------

Open the terminal and execute the following command:

```sh
bash <(curl -s https://raw.githubusercontent.com/pagopa/developer-laptop/master/laptop)
```

**Once the script is done, quit and relaunch Terminal.**

Things We'd like to include in the future
-------
* configure OSX trackpad and gestures settings
* setup ssh keys 
* ensure idempotency (that is: you can run the same script on a non-blank system to restpre setup)
* let users decide what to install and what don't


Credits
-------

This laptop script is inspired by
[thoughbot's laptop](https://github.com/thoughtbot/laptop) script.

### Public domain

thoughtbot's original work remains covered under an [MIT License](https://github.com/thoughtbot/laptop/blob/c997c4fb5a986b22d6c53214d8f219600a4561ee/LICENSE).

Our work on this project is in the worldwide [public domain](LICENSE.md), as are contributions to our project. As stated in [CONTRIBUTING](CONTRIBUTING.md):

> This project is in the public domain within the United States, and copyright and related rights in the work worldwide are waived through the [CC0 1.0 Universal public domain dedication](https://creativecommons.org/publicdomain/zero/1.0/).
>
> All contributions to this project will be released under the CC0 dedication. By submitting a pull request, you are agreeing to comply with this waiver of copyright interest.
