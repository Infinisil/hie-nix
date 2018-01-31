Note: this is a WIP document, once usage is agreed, it will be
implemented using https://github.com/input-output-hk/stack2nix

# Purpose

The purpose of this repository is to provide [HIE](https://github.com/haskell/haskell-ide-engine)
for each major GHC version installable via Nix.

Hie built with specific GHC needs to match the major version of GHC used on development project.


# Install

    $ git clone https://github.com/domenkozar/hie-nix.git
    $ nix-env -f hie-nix -i hies

# Usage

    $ hie-8.0 --help
    $ hie-8.2 --help


To follow discussion how correct version of hie is picked per project, read https://github.com/haskell/haskell-ide-engine/issues/439#issuecomment-359801662
