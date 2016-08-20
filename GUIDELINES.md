# Guidelines For New Projects

## Hello
Welcome to the team! We're happy you're here and look forward to the amazing software you'll build with us.

We value [Convention over Configuration][cc] and use a standard application architecture across all our projects. 

Unless specified otherwise, please follow these guidelines for all new projects.

[cc]: https://en.wikipedia.org/wiki/Convention_over_configuration

## Start With This Repo
We use this [Base Repo][br] to standardize our application architecture. Please review [README.md][rm] for details on each file and folder in the Base Repo.

[br]: https://github.com/dperuo/base-repo
[rm]: https://github.com/dperuo/base-repo/blob/master/README.md

## Use Vagrant
We use Vagrant to standardize our development environment across computers. Please follow Best Practice for working with Vagrant projects.

## Use Git and Github Flow
We use Git and [Github Flow][ghf] as our version control system. Please follow Best Practice for working with Git and Github Flow.

[ghf]: https://github.com/dperuo/base-repo/blob/master/CONTRIBUTING.md

## Use npm
We use npm as our package manager and task runner. Please follow Best Practice for working with npm modules and `npm run` scripts.

## Use Travis CI
We use Travis CI as our integration server of choice. Please follow Best Practice for working with Travis CI.

## Use Angular 2
Angular is our JavaScript framework of choice. Use [Angular 2][a2] unless [Angular 1][a1] is asked for by name.

[a1]: https://angularjs.org/
[a2]: https://angular.io/

## Use Jasmine, Karma and Protractor
Jasmine, Karma and Protractor are our test frameworks of choice. Please follow Best Practice for Jasmine, Karma and Protractor testing.

## Use SCSS
We use SCSS as our CSS pre-processor. Please follow Best Practice for working with SCSS files.

## Use BEM for CSS
We use BEM syntax for all CSS class names. Please follow Best Practice for working with BEM syntax.

## Use JSDoc and TypeDoc
We use [JSDoc][jsd] and [TypeDoc][tsd] as our documentation system. Please follow Best Practice for writing JSDoc and TypeDoc files.

[jsd]: https://github.com/jsdoc3/jsdoc
[tsd]: https://github.com/TypeStrong/typedoc

# Use Bootstrap for Sass
[Bootstrap for Sass][bs] is our CSS framework of choice. Please follow Best Practice for working with Bootstrap.

[bs]: https://github.com/twbs/bootstrap-sass

## Use Atomic Design
All components should be self contained and follow [Unix philosophy][up]:

1. Each module and component does "one thing well."
1. Large complex modules and components build on top of small simple modules and components.
1. All modules and componenets must be "plug-and-play" ready: Adding new modules and componenets to a project must be as simple as importing the appropriate file or folder and wiring it into the project.

[up]: https://en.wikipedia.org/wiki/Unix_philosophy

## Use Zero-Based Indexing
Lists and indexes should always start with zero. For example, the existence of `dev_server_01` implies the existance of `dev_server_00`.
