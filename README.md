# Purpose

The purpose of this repository is to provide [HIE](https://github.com/haskell/haskell-ide-engine)
for each major GHC version installable via Nix.

Hie built with specific GHC needs to match the major version of GHC used on development project.


# Install

    $ git clone https://github.com/domenkozar/hie-nix.git
    $ nix-env -f hie-nix -iA hies

Or for just a specific GHC:

    $ nix-env -f hie-nix -iA hie82

# Usage

    $ hie-8.0 --help
    $ hie-8.2 --help

# Updating HIE

    $ ./update.sh

# FAQ

## How do I make editor integrate the right hie version?

To follow discussion how correct version of hie is picked per project, read https://github.com/haskell/haskell-ide-engine/issues/439#issuecomment-359801662

## Does hie-nix work with Stack?

Yes, but make sure you have Nix enabled in either `stack.yaml` in your project or globally:

    $ cat ~/.stack/config.yaml
    nix: 
      enable: true

