# Helpers

[![license](https://img.shields.io/github/license/janikarh/helpers)](https://github.com/janikarh/helpers/blob/master/LICENSE)

Various CLI helper tools for the daily life on the Terminal.

[A changelog](CHANGELOG.md) is maintained.

## Prerequisites

This has been built for and tested on `macOS catalina 10.15.4`, `zsh` and `Python3.6+`. This might work on other environments too, or not.

**Important:** In your `~/.zshrc` set a new environment variable `HELPERS_HOME` (`export HELPERS_HOME="[full-path-to-the-helpers-location-without-trailing-slash]"`).

## Helpers available

1. [Scaffold new Project](#scaffold-new-project)


## Scaffold new Project

Installation is as easy as adding the following to your `.zshrc`:
`alias scaffold=". [full-path-to-the-helpers-location]/scaffold.sh"`

After sourcing with `source ~/.zshrc`, simply run `scaffold` and follow the prompt.

### Project template alternatives

At the moment, there are the following project options available.

Common actions for all alternatives:

1. Creates a new project directory, under current directory.
2. Optionally initializes *a new git repository* to project directory.

#### Python_Basic

Scaffold a basic Python project based on the system-level Python version (whatever `python3` returns).

1. Creates *an virtual environment* named `venv` within the project directory, and activates it.
2. Installs the latest versions of `pip` and `setuptools` as *production dependencies*, and `flake8` as *a development dependency* to the *venv*.
3. Writes and **pins** the versions of the previous packages to `requirements.txt` and `requirements-dev.txt` respectively.
4. Copies *starter files* from `templates/Python_Basic` to project directory.


#### Python_AWS_Serverless

Does not do anything, at the moment :) Consider this a placeholder.
