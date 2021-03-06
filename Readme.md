## CSSketch - CSS for Sketch 3
CSSketch is a Sketch 3 plugin that enables you to modify your designs quickly by attaching it a stylesheet to it that you can use to lay out your designs, change colors and shadows quickly, etc.
It supports [{less}](http://lesscss.org) stylesheets, which means you can put functions and variables in your stylesheet to make your workflow even more efficient.

CSSketch is completely open source, so feel free to contribute to its development!

## The Story Behind CSSketch
#### [Programmers Design Differently: Why I Built a CSS Plugin for Sketch 3](https://medium.com/@punksomething/programmers-design-differently-why-i-built-a-css-plugin-for-sketch-3-52a1246305a4) on Medium.com

## Screencast

![Screencast](https://raw.githubusercontent.com/JohnCoates/CSSketch/master/screencast.gif)

## Download & Install
Download from [Github](https://github.com/JohnCoates/CSSketch/archive/master.zip)

Two ways to install:

**Option A:** Open CSSketch.sketchplugin and Sketch will ask if you'd like it installed

**Option B:** While Sketch 3 is open, go to Plugins -> Reveal Plugins Folder, and place CSSketch.sketchplugin there.

## Using CSSketch

* To enable CSSketch you must run the menu bar option every time Sketch 3 launches. You can find it on the menu bar at Plugins -> CSSketch -> Layout Layers.
* A stylesheet is set on a per-page basis. Set the stylesheet at Plugins -> CSSketch -> Set Page's Stylesheet for every page you want a stylesheet for. Once this is set, simply make changes to the stylesheet and save them to see the effects.
* Take a look in Examples/ for examples of what you can do right now.
* **Please Note:** Handling for many CSS rules is missing currently.


## Features
* **Less Support:** Variables and functions are supported. Find out more at [LessCSS.org](http://lesscss.org)
* **Auto Detect Stylesheet changes:** Set the stylesheet once, and that's it. Changes are detected and applied as soon as you save the stylesheet.
* **Webkit Engine:** CSSketch is powered by the WebKit engine, the same code that powers Safari and Google Chrome.
* **Toolbar Icon:** A toolbar icon is added after running CSSketch for easy applying of changes.
* **Sandbox Support:** CSSketch works with the Mac App Store version of Sketch 3 as well as the regular version.
* **Stylesheet Path Store In Document:** You only ever have to set the stylesheet path once. It's then stored in the document for future use.

## Supported CSS
* CSSketch uses the system version of WebKit. Upgrade to El Capitan for the best compatibility with CSS standards.
* All layout variables should work fine.
* All elements are given default values of position:absolute, top, and left, with their current positions on the artboard.
* For selectors: All layers are the element type "layer". The name attribute is set to a layer's name, minus the classes. The type attribute is set to "text" for text, and "artboard" for artboards.
* Background-color is supported
* Border is supported (only solid lines)
* Shadow is supported
* Color is supported
* Text-transform is supported


## Community
- **Find a bug?** [Open an issue](https://github.com/JohnCoates/CSSketch/issues/new). Try to be as specific as possible.
- **Have a feature request** [Open an issue](https://github.com/JohnCoates/CSSketch/issues/new). Tell me why this feature would be useful, and why you and others would want it.

## Contribute
Lot of CSS rules have yet to be added. They're decently easy to add. I appreciate all pull requests! You'll want to modify the following files to add CSS rule handling:
* CSS Rule handlers: [CSSketch Helper/src/Models/Layout/CSKLayerCSS.m](https://github.com/JohnCoates/CSSketch/blob/master/CSSketch%20Helper/src/Models/Layout/CSKLayerCSS.m)
* Sketch Header Stubs: [CSketch Helper/src/Headers/CSSketchHeaders.h](https://github.com/JohnCoates/CSSketch/blob/master/CSSketch%20Helper/src/Headers/CSKSketchHeaders.h)

## Changelog

- October 2015 - 1.0: first release

## License
[MIT License](https://raw.githubusercontent.com/JohnCoates/CSSketch/master/LICENSE)

## Author
Maintained and created by John Coates [@punksomething](http://twitter.com/punksomething)
