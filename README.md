# demo-fvttdev-module
Provides a demo of using `fvttdev`, a zero config CLI, to bundle a module for Foundry VTT

Please note that `fvttdev` is presently in alpha though has been released and this repo shows essential usage for 
the `bundle` command. In short the `fvttdev` bundle command captures all of the functionality configured in 
[demo-rollup-module](https://github.com/typhonjs-fvtt/demo-rollup-module) with several additions like Typescript 
support and Babel for transformation of the latest JS 2020/1 code.

This demo is very simple and open a dialog box showing a unique name generator when you launch a scene. It works on 
Foundry 0.7.x and 0.8.x.

- clone repo
- update the deploy paths in the `./env` files to point to a new folder in your FoundryVTT-Data modules directory
called `demo-fvttdev-module`.
- npm run bundle-deploy  (this is the `./env/deploy.env) file. 
- npm run show-bundle-help for help

As of 05.28.21 all underlying tooling is the latest released versions including Typescript 4.3.2, Babel, PostCSS w/ 
Sass, Less, Stylus support out of the box.

More to come for sure. Please refer to `demo-rollup-module` linked above to get an idea of what is involved. The 
big difference with `fvttdev` is that it is all zero config though you can define config files for the various tooling
if desired. 
