#**React**(with **JSX**) + **Backbone** + **Require** project snippet.

Building of project is managed with **grunt**, testing with **karma** and **Jasmine**.

## How to start (*nix)
* `git clone https://github.com/iLikeKoffee/backreact YOUR_PROJECT_DIRECTORY`
* `cd YOUR_PROJECT_DIRECTORY`
* `chmod +x install-deps.sh`
* `chmod +x install-env.sh`
* `sh ./install-env.sh` *Requires root access*, if you have bower, grunt and grunt-cli installed, skip it.
* `sh ./install-deps.sh` *Should work without root access.*
* `grunt` - Should run do some work on building examples, run tests in Chrome(Chrome window will blink once) and open working examples in your default browser.
* `git remote remove origin` and `git remote add origin YOUR_REPO_URL` - change origin from this repo to your one.
* `git push origin master --set-upstream` 

## Implemented grunt commands
* `grunt`, `grunt serve` - start connect server and rebuild project on every change.
* `grunt lint` - check code style of .js and .jsx files.
* `grunt clean` - remove all build results.
* `grunt build` - build project(clean, then lint, then compile less and jsx, then run all tests).
* `grunt test` - run project tests in chrome browser. *PhantomJS doesn't work yet.*

## Examples
* app/scripts/router.js - Routing file.
* app/scripts/ui-components/src/panel/panel.jsx - example of defining UI component.
* app/scripts/controllers/src/*.jsx - example of defining controllers.
* test/ui-components/src/panel.test.jsx - example of testing react components in .jsx syntax.

## Plans
* Write controllers test example.
* Implement yoman scaffolding.
* Implement `grunt dist` command to minify all code and build ready-to-deploy distribution.

## List of production dependencies(bower)
* backbone ~1.1.2
* bootstrap ~3.3.2
* jquery ~2.1.3
* react.backbone ~0.6.0
* react ~0.12.2
* requirejs ~2.1.15

## List of development dependencies(npm)
* bower
* grunt
* a lot of grunt plugins
* karma
* jasmine-core
* karma-jasmine
* karma-chrome-launcher
* requirejs
* karma-requirejs
* react-tools
* npm