# Onboarding For Developers At Fixate

Below you'll find a list of tools, processes, and general things we do and use at Fixate.

## Command Line

- [Larry's dotfiles](https://github.com/larrybotha/dotfiles) for automated setup of local environment

## Git

- [BitBucket](http://bitbucket.org) for private repos
- [Git Flow](http://danielkummer.github.io/git-flow-cheatsheet/) as our git branching model
  - work is branched off of develop
  - feature branches are for features that are being worked on
    - features should be small portions of work, usually no more than 2 days of work at a time
    - always branched off of develop
  - hotfixes are for quick fixes that need to be in master quickly
    - are branched from master, merged into master and develop
    - tagged as 0.0.x (i.e. a patch)
  - release branches are preparation for a major release
    - are branched from develop, and merged into both master and develop
    - tagged as 0.x.0 or x.0.0 depending on size if a major or minor release
