# jsFiddle Plugin for Octopress

## History (Or, WTF am I hosting this, when it's built into Octopress?)

This plugin was originally written by [Brian Arnold](https://github.com/brianarn) (his original post about it [can be found here](http://brianarn.github.com/blog/2011/08/jsfiddle-plugin/), and has since been incorporated into the Octopress core. However, [Brandon Mathis (imathis)](https://github.com/imathis), the creator of Octopress, mentioned [in a recent pull request](https://github.com/imathis/octopress/pull/789) that the jsFiddle plugin (and I suspect a good number of plugins) is being dropped from Octopress 2.1.

Since Brian no longer has the plugin as one of his own repositories -- and because I've made some modifications -- I've decided to give it a home and make a sort of pseudo-fork of the plugin, in preparation for Octopress removing the plugin from core.

## Improvements on the original

The original script itself is pretty simple and works as intended (in part thanks to the straightforwardness of jsFiddle's <del>API</del> embedding capabilities) for basic Fiddles. However, I found myself wanting to use jsFiddle's versioning system to display changes in a given sample. I also ran into problems with the built URL effectively stripping out my username.

A quick search turned up the aforementioned pull request, but both the people involved in the conversation only had whatever changes they made to their Octopress install as a whole in their Octopress repository. 

With the help of [Zach Thomae's](https://github.com/zthomae) code in the pull request, I've updated the plugin to allow for any one of the following variations:

- shorttag
- username/shorttag
- shorttag/revision
- username/shorttag/revision

## Usage

Usage is exactly the same, except now, instead of just putting `yzfH2` in the tag, you can put in `[username]/yzfH2`, `yzfH2/1`, or even `[username]/yzfH2/1`.
