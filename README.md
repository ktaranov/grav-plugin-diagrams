# Grav Diagrams Plugin

`sequence` is a [Grav](http://github.com/getgrav/grav) plugin that adds simple and powerful sequence diagram functionality utilizing the Javascript plugin [js-sequence-diagrams](https://bramp.github.io/js-sequence-diagrams).

# Installation

Installing the Diagrams plugin can be done with the manual method enables you to do so via a zip file. 

## Manual Installation

To install this plugin, just download the zip version of this repository and unzip it under `/your/site/grav/user/plugins`. Then, rename the folder to `diagrams`. You can find these files either on [GitHub](https://github.com/getgrav/grav-plugin-highlight).

You should now have all the plugin files under

    /your/site/grav/user/plugins/diagrams

>> NOTE: This plugin is a modular component for Grav which requires [Grav](http://github.com/getgrav/grav) and a theme to be installed in order to operate.

# Usage

The plug-in is configured to be functional as soon as you finished installation. To use it in an item of your site, you just have to write your sequence diagram as follows:

eg:

    [sequence]
	A->B:Hi C for me !
	B-->A:With pleasure
	B->C:A says hello
	[/sequence]

The plugin will transform this sequence to display the following diagram:

<p align="center">
  <img src="assets/sequence.png" width="350"/><br/>
  <i>Created diagram</i>
</p>

# Settings

You can parameterize the plugin to suit your usage

| Name     | Value        | Use   |
| -------- |:------------:| -----:|
| enabled  | true / false | plugin activation |
| theme    | simple / hand | diagram theme |
| align    | left / center / right | diagrams position |

# Updating

As development for the Diagrams plugin continues, new versions may become available that add additional features and functionality, improve compatibility with newer Grav releases, and generally provide a better user experience. Updating Diagrams is easy, and can be done through manually.

## Manual Update

Manually updating Diagrams is pretty simple. Here is what you will need to do to get this done:

* Delete the `your/site/user/plugins/diagrams` directory.
* Downalod the new version of the Highlight plugin from either [GitHub](#).
* Unzip the zip file in `your/site/user/plugins` and rename the resulting folder to `diagram`.
* Clear the Grav cache. The simplest way to do this is by going to the root Grav directory in terminal and typing `bin/grav clear-cache`.