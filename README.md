:toc: preamble
:project_name: Project Foobar
:ci_badge: image:https://travis-ci.org/dperuo/riker-ipsum.svg?branch=master["Build Status", link="https://travis-ci.org/dperuo/riker-ipsum"]
ifdef::env-github[]
:caution-caption: :fire:
:important-caption: :heavy_exclamation_mark:
:note-caption: :dart:
:tip-caption: :bulb:
:warning-caption: :warning:
endif::[]

= {project_name}

{ci_badge}

Welcome to {project_name}! This README is the central hub for all project documentation. It's a living document that updates often. Please review and change it as needed.

== System Requirements

.Required
[horizontal]
Angular CLI:: 1.0.0 or higher
Homebrew:: 1.1.12 or higher
Node.js:: 7.7.1 or higher
npm:: 4.2.0 or higher
Vagrant:: 1.9.3 or higher
VirtualBox:: 5.1.18 or higher
Yarn:: 0.22.0 or higher

.Recommended
[horizontal]
Google Chrome:: 57 or higher

== Quick Start

```
cd path/to/local/repos
git clone git@github.com:Foobar/foobar-ABC.git foobar-ABC
cd ./foobar-ABC
./.foobootstrap
./.foostart
```

View your local build at `http://192.168.10.89/`.

NOTE: You may need root access for `.foobootstrap` and `.foostart`.

== Project Architecture

[horizontal]
`@deployment/`:: Folder for all CI and CD scripts
`@docs/`:: Folder for all project documentation
`@provisioning/`:: Folder for all environment provisioning scripts
`e2e/`:: All integration and end-to-end tests for the ABC app
`src/`:: All source code for the ABC app
`.angular-cli.json`:: Config file for Angular CLI
`.foobootstrap`:: Script to set up new local development environments
`.foobuild`:: Build a deployable app without watching for changes
`.foostart`:: Launch a local development environment and watch for changes
`.footest`:: Run the full test suite against your build without watching for changes
`.editorconfig`:: Config file for EditorConfig
`.gitignore`:: Git ignore file for this project
`.gitmessage`:: Git commit message template this project
`.travis.yml`:: Config file for Travis CI
`README.md`:: This file
`Vagrantfile`:: Config file for Vagrant
`karma.conf.js`:: Config file for Karma
`package.json`:: Config file for Yarn
`protractor.conf.js`:: Config file for Protractor
`tsconfig.json`:: Config file for TypeScript
`tslint.json`:: Config file for TSLint
`yarn.lock`:: Lock file for Yarn

NOTE: Always prefix folders not directly related to the Angular app with `@`. This helps distinguish between 'application' files and 'application support' files.

== Documentation

[horizontal]
link:./@docs/API.md[`API.md`]:: Logs all available REST requests and their responses
link:./@docs/DIRECTORY.md[`DIRECTORY.md`]:: Lists who's who on the team
link:./@docs/ELSE.md[`ELSE.md`]:: Documentation for the larger team
link:./@docs/FLAGS.md[`FLAGS.md`]:: How to use Feature Flags in this project
link:./@docs/PLAYBOOK.md[`PLAYBOOK.md`]:: Details how we like to work at foobar ABC
link:./@docs/ROADMAP.md[`ROADMAP.md`]:: Outlines our long-term plan and direction for this project
link:./@docs/STYLEGUIDE.md[`STYLEGUIDE.md`]:: Defines DOs and DON'Ts when writing code

== Development

All development is done on the `master` branch (details here). Use link:./@docs/FLAGS.md[feature flags] to show and hide functionality and UI.

Test your code locally before pushing to Github.

`master` is the only branch tested on Travis CI and pushed into production.

`master` is always the Source of Truth for the current state of ABC.

Use feature branches with caution. Feature branches are always personal, temporary, and must be deleted as soon as they are merged back into `master`.

Develop and test directly on the `master` branch when in doubt.

Use the Angular CLI tool to scaffold new code. Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive/pipe/service/class/module`.

Use the `.foo*` family of custom scripts for common developer tasks:

[horizontal]
`.foobuild`:: Build a deployable app without watching for changes
`.foostart`:: Launch a local development environment and watch for changes
`.footest`:: Run the full test suite against your local build without watching for changes

NOTE: The `.foo*` family of scripts is a new convention used in a few CAT Team projects to streamline and standardize local development environment setup. Expect more projects to use this convention in the future.

This app uses the https://github.com/Foobar/foobar-ionic-components[foobar Components] repo for its component library. If you are not actively working on foobar Components, can easily install and update the dependency using Yarn:

```
cd path/to/local/foobar-ABC
yarn add Foobar/foobar-components
.foostart
```

NOTE: You must run `yarn upgrade Foobar/foobar-components` every time the foobar Components library updates if you use this method.

If you are actively working on foobar Components we recommend using `yarn link` so you can develop both repos at the same time:

```
cd path/to/local/repos
git clone git@github.com:Foobar/foobar-components.git foobar-components
cd ./foobar-components
yarn link
cd to/your/local/foobar-ABC
yarn link foobar-components
```

NOTE: You must watch for changes in both `foobar-components` and `foobar-ABC` during active development.

== Testing

The test suite gives developers a high level of confidence when building new features and fixing bugs. It's okay if we have less than 100% coverage as long as developer condiance is high.

== Deployment

Please read the link:./@docs/DEPLOYMENT.md[documentation] for details.


# Browser and Hardware Support

ABC follows Foobar Engineering's official guidelines for browser support:

OS X::
* Latest release of Chrome
* Latest release of Firefox
* Latest release of Safari

Windows::
* Edge
* IE 10
* IE 11
* Latest release of Chrome
* Latest release of Firefox

iOS::
* Latest and previous version of iPad
* Latest and previous version of iPhone
* Latest release of Safari

Android 4.1+::
* Latest release of Chrome
* Latest release of Firefox
