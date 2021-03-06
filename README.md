
<p align="center"><a href="https://giojs.org" target="_blank"><img width="100" src="https://github.com/syt123450/giojs/blob/master/assets/readme/logo.png" alt="Gio logo"></a></p>

<h1 align="center">Gio.js</h1>

<p align="center">
<strong>English</strong> | <a href="https://github.com/syt123450/giojs/blob/master/README_zh.md"><strong>中文</strong></a>
</p>

<p align="center">React Version: <a href="https://github.com/syt123450/react-giojs">react-giojs</a></p>

<p align="center">
  <a href="https://www.npmjs.com/package/giojs"><img src="https://img.shields.io/npm/v/giojs.svg" alt="npm version" height="18"></a>
  <a href="https://github.com/syt123450/Gio.js/blob/master/LICENSE"><img src="https://img.shields.io/badge/license-Apache--2.0-green.svg" alt="license badge"></a>
  <a href="https://github.com/mrdoob/three.js/"><img src="https://img.shields.io/badge/dependencies-Three.js-brightgreen.svg" alt="dependencies badge"></a>
  <a href="https://travis-ci.org/syt123450/Gio.js"><img src="https://travis-ci.org/syt123450/Gio.js.svg" alt="build"></a>
  <a href="https://coveralls.io/github/syt123450/Gio.js?branch=master"><img src="https://coveralls.io/repos/github/syt123450/Gio.js/badge.svg" alt="coverage"></a>
</p>

**Gio.js** is an open source library for web 3D globe data visualization built with Three.js. What makes Gio.js different is that it is **simple** to use Gio.js to **customize** a 3D data visualization model in a declarative way, add your own data, and integrate it into your own **modern** web application.

<!-- [START screenshot] -->
<p align="center">
  <img src="https://github.com/syt123450/giojs/blob/master/assets/readme/Gio.gif"/>
</p>
<!-- [END screenshot] -->

## Content

* [Motivation](#motivation)
* [Getting Started](#getting-started)
* [Examples](#examples)
* [Documentation](#documentation)

<!-- [START motivation] -->

## Motivation

**Gio.js** is an open source library for web 3D globe data visualization built with Three.js. What makes Gio.js different is that it is **simple** to use Gio.js to **customize** a 3D data visualization model in a declarative way, add your own data, and integrate it into your own **modern** web application.

This library is inspired by the <a href="https://github.com/dataarts/armsglobe">Arms Trade Visualization project</a> developed by Michael Chang and presented during Google Ideas INFO 2012. See <a href="http://mflux.tumblr.com/post/28367579774/armstradeviz">original post</a>. With Gio.js, it is easy to reproduce this fantastic data visualization model, and integrate it into web application.

* **Simplicity** -- Create a 3D global data visualization model with your own data in just four lines of javascript code
* **Customization** -- Design your own globe style with easy to use APIs in Gio.js
* **Modernization** -- Build a responsible, fully interactive, rich 3D frontend application using Gio.js

<!-- [END motivation] -->

<!-- [START getstarted] -->
## Getting Started

### Installation
- Option 1: \<script\> tag

Include Three.js dependency:
```html
<script src="three.min.js"></script>
```
Include local Gio.js library
```html
<script src="gio.min.js"></script>
```
or through CDN
```html
<script src="https://threejs.org/build/three.min.js"></script>
<script src="https://raw.githack.com/syt123450/giojs/master/build/gio.min.js"></script>
```
- Option 2: npm
```bash
npm install giojs --save
```
- Option 3: yarn
```bash
yarn add giojs
```
### Usage

After including "three.min.js" and "gio.min.js" in your html, create a `div` to render the 3D Gio globe:

```html
<!DOCTYPE HTML>
<html>
<head>

  <!-- include three.min.js library-->
  <script src="three.min.js"></script>

  <!-- include gio.min.js library-->
  <script src="gio.min.js"></script>

</head>
<body>

  <!-- container to draw 3D Gio globe-->
  <div id="globalArea"></div>

</body>
</html>

```
To initialize and render the 3D Gio globe:

```html

<script>

    // get the container to hold the IO globe
    var container = document.getElementById( "globalArea" );

    // create controller for the IO globe, input the container as the parameter
    var controller = new GIO.Controller( container );

    // use addData() API to add the the data to the controller, know more about data format check out documentation about data: http://giojs.org/html/docs/dataIntro.html
    controller.addData( data );

    // call the init() API to show the IO globe in the browser
    controller.init();

</script>
```
If everything goes well, you shall see [this](http://giojs.org/examples/00_hello_world(simplest).html). For more fancier usage of Gio.js, check out <a href="http://giojs.org/html/docs/index.html">Gio.js API document</a>

Click the codepen logo to try it in Codepen: &nbsp;&nbsp;<a target="_blank" href="https://codepen.io/syt123450/pen/VXNdgM"><img width=50 height=50 src="https://rawgit.com/syt123450/Gio.js/master/assets/readme/codepen.png"></a>

<!-- [END getstarted] -->

<!-- [START documentation] -->

## Examples

Gio.js has many representative demos to show how to work with Gio.js, there are mainly three example resources:

- **Resource 1**: Gio.js Playground

There is a Playground ( <a href="http://giojs.org/html/playground.html">playground link</a> ) for developers to play with Gio.js and export Gio.js parameter.

- **Resource 2**: Github "examples" folder

Gio.js has many API demos, and these demos are gathered in examples folder. clone the Gio.js repo, try them in your own environment ~

- **Resource 3**: Live demos on Codepen

Gio.js has a Codepen collection which contains many live demos about Gio.js, click the codepen logo and try to edit them!
<a target="_blank" href="https://codepen.io/collection/DkBobG/"><img width=50 height=50 src="https://rawgit.com/syt123450/Gio.js/master/assets/readme/codepen.png"></a>

## Documentation

- For quick start, see [Getting Started](https://github.com/syt123450/Gio.js/blob/master/docs/en/Getting_Started.md)
- To learn more about the [Basic Elements](https://github.com/syt123450/Gio.js/blob/master/docs/en/Basic_Elements.md)
- To see the full API document in Markdown format, see [APIs](https://github.com/syt123450/Gio.js/blob/master/docs/en/APIs.md)
- To contribute to Gio.js's code base, read [Developer Guide](https://github.com/syt123450/Gio.js/blob/master/docs/en/Developer_Guide.md)
- See Gio's official website [giojs.org](http://giojs.org) for everything above and plus lots of live examples
<!-- [END documentation] -->


[screenshot-url]: http://via.placeholder.com/400x300
[npm-badge]: https://img.shields.io/badge/npm-v0.0.5-orange.svg
[npm-badge-url]: https://www.npmjs.com/package/giojs
[license-badge]: https://img.shields.io/badge/license-MIT-brightgreen.svg
[license-badge-url]: https://github.com/syt123450/Gio.js/blob/master/LICENSE
[dependencies-badge]: https://img.shields.io/badge/dependencies-Three.js-brightgreen.svg
[dependencies-badge-url]: https://github.com/mrdoob/three.js/
