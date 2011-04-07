## pairs

This script will read a .pairs file and create pairings for you.

## Commands

Available commands:

    pairs help
      - show commands and .pairs file syntax

    pairs list
      - gives a list of names and initials from a .pairs file

    pairs make [sm tp ...]
      - creates a random pairing based on a .pairs file
      - if initials are provided, only uses those people


The .pairs file format and this code is based on [pivotal's git-scripts](https://github.com/pivotal/git_scripts)

## Setup

You'll need to create a `.pairs` config file to map initials to names and email ids.  The example file:

    # .pairs - configuration for 'git pair'
    # place in project or home directory
    pairs:
      eh: Edward Hieatt
      js: Josh Susser; jsusser
      sf: Serguei Filimonov; serguei
    email:
      prefix: pair
      domain: pivotallabs.com

You can put the .pairs file in your project repo root directory and check it into git, or you can put it in your ~ directory so it's available to all projects on the workstation.
