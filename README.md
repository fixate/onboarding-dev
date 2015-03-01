# Onboarding For Developers At Fixate

Below you'll find a list of tools, processes, and general things we do and use at Fixate.

## Command Line

- [Larry's dotfiles](https://github.com/larrybotha/dotfiles) for automated setup of local environment (Mac OSX)
- [Rsync](https://www.digitalocean.com/community/tutorials/how-to-use-rsync-to-sync-local-and-remote-directories-on-a-vps) and [SSH](https://help.github.com/articles/generating-ssh-keys/) for CMS deployment
  - [quickly adding SSH keys to a remote server](https://gist.github.com/7786195)

## Git

- Intro to [Git](https://www.codeschool.com/courses/try-git)
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
- [GistBox](https://app.gistboxapp.com/library/my-gists) for easy Github gist management

## Editing

- [Sublime Text](http://www.sublimetext.com/)
- [editorconfig](http://editorconfig.org/) consistent indentation, line ends, etc. for all team members

## Task Automation

- [Gulp](gulpjs.com)
  - [Fixate's ProcessWire gulpfile](https://github.com/fixate/generator-fixate-pw/blob/develop/app/templates/_gulpfile.coffee)
- [Yeoman Generators](http://yeoman.io/generators/) for quickly generating projects
  - used to generate [ProcessWire pojects](https://github.com/fixate/generator-fixate-pw/)

## CSS

- [Sass](http://sass-lang.com/) for preprocessing CSS
- Familiarity with the following authors and techniques for modular and scalable CSS:
  - [Harry Robert's Blog](http://csswizardry.com)
  - [BEM Methodology](https://en.bem.info/method/)
  - [SMACSS](https://smacss.com/)

## Javascript

- [CoffeeScript](http://coffeescript.org/) for preprocessing JS
- [Javascript Is Sexy](javascriptissexy.com)
- [Eloquent Javascript](http://eloquentjavascript.net/)
- [Javascript Design Patterns](http://addyosmani.com/resources/essentialjsdesignpatterns/book/)

## CMS

- [ProcessWire](http://processwire.com)

## Favicons

- [X-Icon Editor](http://www.xiconeditor.com/) for multi-layered favicons that are crisp on all devices

## Font Icons

- [IcoMoon](http://icomoon.com/app) for generating icon files from raw vector images

## Cutting Up Designs

- [Adobe Illustrator Basics](https://www.udemy.com/learn-adobe-illustrator-from-scratch/)
- images to always be on artboards with even widths and heights
  - scaling is better on even numbers
- artboards to always be on whole number pixels
  - reduces anti-aliasing on file save
- photographs always saved as jpeg / jpg
  - [JpegMini](http://jpegmini.com) for optimisation
- images with fewer than 1 million colours and/or transparency saved as png 24
- images with fewer than 256 colours and no transparency saved as png 8
- pngs and svgs minified via gulp tasks
