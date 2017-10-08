# Bootstrap

## Bootstrap

**Bootstrap is the most popular HTML, CSS, and JS framework for developing responsive, mobile first projects on the web.**

*Currently v3.3.7*

### Designed for everyone, everywhere

Bootstrap makes front-end web development faster and easier. It's made for folks of all skill levels, devices of all shapes, and projects of all sizes.
Sass and Less support

#### Preprocessors

Bootstrap ships with vanilla CSS, but its source code utilizes the two most popular CSS preprocessors, Less and Sass. Quickly get started with precompiled CSS or build on the source.
Responsive across devices

#### One framework, every device.

Bootstrap easily and efficiently scales your websites and applications with a single code base, from phones to tablets to desktops with CSS media queries.
Components

#### Full of features

With Bootstrap, you get extensive and beautiful documentation for common HTML elements, dozens of custom HTML and CSS components, and awesome jQuery plugins.

*Bootstrap is open source. It's hosted, developed, and maintained on GitHub.*

[Github](https://github.com/twbs/bootstrap)

### Official Bootstrap Themes

Take Bootstrap to the next level with official premium themes. Each theme is its own toolkit featuring all of Bootstrap, brand new components and plugins, full docs, build tools, and more.

[Browse themes](https://themes.getbootstrap.com/)

### Built with Bootstrap

Millions of amazing sites across the web are being built with Bootstrap. Get started on your own with our growing [collection of examples](https://getbootstrap.com/docs/getting-started/#examples) or by exploring some of our favorites.

* [Lyft](http://expo.getbootstrap.com/2014/10/29/lyft/)
* [Vogue](https://getbootstrap.com/assets/img/expo-vogue.jpg)
* [Riot Design](https://getbootstrap.com/assets/img/expo-riot.jpg)
* [Newsweek](http://expo.getbootstrap.com/2014/02/12/newsweek/)

We showcase dozens of inspiring projects built with Bootstrap on the Bootstrap Expo.

[Explore the Exop](http://expo.getbootstrap.com/)

-------------------------------------------------------------------------------

## Getting started

**An overview of Bootstrap, how to download and use, basic templates and examples, and more.**

### Download

Bootstrap (currently v3.3.7) has a few easy ways to quickly get started, each one appealing to a different skill level and use case. Read through to see what suits your particular needs.

##### Bootstrap

Compiled and minified CSS, JavaScript, and fonts. No docs or original source files are included.

[Download](https://github.com/twbs/bootstrap/releases/download/v3.3.7/bootstrap-3.3.7-dist.zip)

##### Source code

Source Less, JavaScript, and font files, along with our docs. Requires a Less compiler and some setup.

[Download](https://github.com/twbs/bootstrap/archive/v3.3.7.zip)

##### Sass

Bootstrap ported from Less to Sass for easy inclusion in Rails, Compass, or Sass-only projects.

[Download](https://github.com/twbs/bootstrap-sass/archive/v3.3.7.tar.gz)

#### Bootstrap CDN

The folks over at [MaxCDN](https://www.maxcdn.com/) graciously provide CDN support for Bootstrap's CSS and JavaScript. Just use these [Bootstrap CDN](https://www.bootstrapcdn.com/) links.


        ```html
	<!-- Latest compiled and minified CSS -->
	<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">

	<!-- Optional theme -->
	<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap-theme.min.css" integrity="sha384-rHyoN1iRsVXV4nD0JutlnGaslCJuC7uwjduW9SVrLvRYooPp2bWYgmgJQIXwl/Sp" crossorigin="anonymous">

	<!-- Latest compiled and minified JavaScript -->
	<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js" integrity="sha384-Tc5IQib027qvyjSMfHjOMaLkfuWVxZxUPnCJA7l2mCWNIpG9mGCD8wGNIcPD7Txa" crossorigin="anonymous"></script>
	```

#### Install with Bower

You can also install and manage Bootstrap's Less, CSS, JavaScript, and fonts using [Bower](http://bower.io/):

        ```shel
	$ bower install bootstrap
	```

#### Install with npm

You can also install Bootstrap using [npm](https://www.npmjs.com/):

        ```shel
	$ npm install bootstrap@3
	```

`require('bootstrap')` will load all of Bootstrap's jQuery plugins onto the jQuery object. The `bootstrap` module itself does not export anything. You can manually load Bootstrap's jQuery plugins individually by loading the **/js/*.js** files under the package's top-level directory.

Bootstrap's `package.json` contains some additional metadata under the following keys:

* `less` - path to Bootstrap's main [Less](http://lesscss.org/) source file
* `style` - path to Bootstrap's non-minified CSS that's been precompiled using the default settings (no customization)

#### Install with Composer

You can also install and manage Bootstrap's Less, CSS, JavaScript, and fonts using [Composer](https://getcomposer.org/):

        ```shel
	$ composer require twbs/bootstrap
	```

#### Autoprefixer required for Less/Sass

Bootstrap uses [Autoprefixer](https://github.com/postcss/autoprefixer) to deal with [CSS vendor prefixes](http://webdesign.about.com/od/css/a/css-vendor-prefixes.htm). If you're compiling Bootstrap from its Less/Sass source and not using our Gruntfile, you'll need to integrate Autoprefixer into your build process yourself. If you're using precompiled Bootstrap or using our Gruntfile, you don't need to worry about this because Autoprefixer is already integrated into our Gruntfile.

### What's included

**Bootstrap is downloadable in two forms, within which you'll find the following directories and files, logically grouping common resources and providing both compiled and minified variations.**

> **jQuery required**
>
>> Please note that *all JavaScript plugins require jQuery* to be included, as shown in the [starter template](https://getbootstrap.com/docs/3.3/getting-started/#template). Consult our **bower.json** to see which versions of jQuery are supported.

#### Precompiled Bootstrap

Once downloaded, unzip the compressed folder to see the structure of (the compiled) Bootstrap. You'll see something like this:

	bootstrap/
	├── css/
	│   ├── bootstrap.css
	│   ├── bootstrap.css.map
	│   ├── bootstrap.min.css
	│   ├── bootstrap.min.css.map
	│   ├── bootstrap-theme.css
	│   ├── bootstrap-theme.css.map
	│   ├── bootstrap-theme.min.css
	│   └── bootstrap-theme.min.css.map
	├── js/
	│   ├── bootstrap.js
	│   └── bootstrap.min.js
	└── fonts/
		├── glyphicons-halflings-regular.eot
		├── glyphicons-halflings-regular.svg
		├── glyphicons-halflings-regular.ttf
		├── glyphicons-halflings-regular.woff
		└── glyphicons-halflings-regular.woff2

This is the most basic form of Bootstrap: precompiled files for quick drop-in usage in nearly any web project. We provide compiled CSS and JS `(bootstrap.*)`, as well as compiled and minified CSS and JS `(bootstrap.min.*)`. CSS [source maps](https://developer.chrome.com/devtools/docs/css-preprocessors) `(bootstrap.*.map)` are available for use with certain browsers' developer tools. Fonts from Glyphicons are included, as is the optional Bootstrap theme.

#### Bootstrap source code

The Bootstrap source code download includes the precompiled CSS, JavaScript, and font assets, along with source Less, JavaScript, and documentation. More specifically, it includes the following and more:

	bootstrap/
	├── less/
	├── js/
	├── fonts/
	├── dist/
	│   ├── css/
	│   ├── js/
	│   └── fonts/
	└── docs/
		└── examples/

The `less/`, `js/`, and `fonts/` are the source code for our CSS, JS, and icon fonts (respectively). The dist/ folder includes everything listed in the precompiled download section above. The docs/ folder includes the source code for our documentation, and `examples/` of Bootstrap usage. Beyond that, any other included file provides support for packages, license information, and development.

### Compiling CSS and JavaScript

**Bootstrap uses [Grunt](http://gruntjs.com/) for its build system, with convenient methods for working with the framework. It's how we compile our code, run tests, and more.**

#### Installing Grunt

To install Grunt, you must first download and [install node.js](https://nodejs.org/download/) (which includes npm). npm stands for [node packaged modules](https://www.npmjs.com/) and is a way to manage development dependencies through node.js.
Then, from the command line:

1. Install `grunt-cli` globally with `npm install -g grunt-cli`.
2. Navigate to the root `/bootstrap/` directory, then run `npm install`. npm will look at the `package.json` file and automatically install the necessary local dependencies listed there.

When completed, you'll be able to run the various Grunt commands provided from the command line.

#### Available Grunt commands

* `grunt dist` (Just compile CSS and JavaScript)
    * Regenerates the `/dist/` directory with compiled and minified CSS and JavaScript files. As a Bootstrap user, this is normally the command you want.
* `grunt watch` (Watch)
    * Watches the Less source files and automatically recompiles them to CSS whenever you save a change.
* `grunt test (Run tests)`
    * Runs [JSHint](http://jshint.com/) and runs the [QUnit](http://qunitjs.com/) tests headlessly in  [PhantomJS](http://phantomjs.org/).
* `grunt docs (Build & test the docs assets)`
    * Builds and tests CSS, JavaScript, and other assets which are used when running the documentation locally via `bundle exec jekyll serve`.
* `grunt` (Build absolutely everything and run tests)
    * Compiles and minifies CSS and JavaScript, builds the documentation website, runs the HTML5 validator against the docs, regenerates the Customizer assets, and more. Requires [Jekyll](http://jekyllrb.com/docs/installation/). Usually only necessary if you're hacking on Bootstrap itself.

#### Troubleshooting

Should you encounter problems with installing dependencies or running Grunt commands, first delete the `/node_modules/` directory generated by npm. Then, rerun npm install.

### Basic template

**Start with this basic HTML template, or modify [these examples](https://getbootstrap.com/docs/3.3/getting-started/#examples). We hope you'll customize our templates and examples, adapting them to suit your needs.**

 the HTML below to begin working with a minimal Bootstrap document.

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="utf-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <!-- The above 3 meta tags *must* come first in the head; any other head content must come *after* these tags -->
        <title>Bootstrap 101 Template</title>
        <!-- Bootstrap -->
        <link href="css/bootstrap.min.css" rel="stylesheet">
        <!-- HTML5 shim and Respond.js for IE8 support of HTML5 elements and media queries -->
        <!-- WARNING: Respond.js doesn't work if you view the page via file:// -->
        <!--[if lt IE 9]>
        <script src="https://oss.maxcdn.com/html5shiv/3.7.3/html5shiv.min.js"></script>
        <script src="https://oss.maxcdn.com/respond/1.4.2/respond.min.js"></script>
        <![endif]-->
    </head>
    <body>
        <h1>Hello, world!</h1>
        <!-- jQuery (necessary for Bootstrap's JavaScript plugins) -->
        <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
        <!-- Include all compiled plugins (below), or include individual files as needed -->
        <script src="js/bootstrap.min.js"></script>
    </body>
    </html>
    ```

### Examples

**Build on the basic template above with Bootstrap's many components. We encourage you to customize and adapt Bootstrap to suit your individual project's needs.**

Get the source code for every example below by [downloading the Bootstrap repository](https://github.com/twbs/bootstrap/archive/v3.3.7.zip). Examples can be found in the `docs/examples/ directory`.

#### Using the framework

![Starter template example]()

**Starter template**

Nothing but the basics: compiled CSS and JavaScript along with a container.

![Bootstrap theme example]()

**Bootstrap theme**

Load the optional Bootstrap theme for a visually enhanced experience.


![Multiple grids example]()

**Grids**

Multiple examples of grid layouts with all four tiers, nesting, and more.

![Jumbotron example]()

**Jumbotron**

Build around the jumbotron with a navbar and some basic grid columns.

![Narrow jumbotron example]()

**Narrow jumbotron**

Build a more custom page by narrowing the default container and jumbotron.

#### Navbars in action

![Navbar example]()

**Navbar**

Super basic template that includes the navbar along with some additional content.

![Static top navbar example]()

**Static top navbar**

Super basic template with a static top navbar along with some additional content.

![Fixed navbar example]()

**Fixed navbar**

Super basic template with a fixed top navbar along with some additional content.

#### Custom components

![A one-page template example]()

**Cover**

A one-page template for building simple and beautiful home pages.

![Carousel example]()

**Carousel**

Customize the navbar and carousel, then add some new components.

![Blog layout example]()

**Blog**

Simple two-column blog layout with custom navigation, header, and type.

![Dashboard example]()

**Dashboard**

Basic structure for an admin dashboard with fixed sidebar and navbar.

![Sign-in page example]()

**Sign-in page**

Custom form layout and design for a simple sign in form.

![Justified nav example]()

**Justified nav**

Create a custom navbar with justified links. Heads up! Not too Safari friendly.

![Sticky footer example]()

**Sticky footer**

Attach a footer to the bottom of the viewport when the content is shorter than it.

![Sticky footer with navbar example]()

**Sticky footer with navbar**

Attach a footer to the bottom of the viewport with a fixed navbar at the top.

#### Experiments

![Non-responsive example]()

**Non-responsive Bootstrap**

Easily disable the responsiveness of Bootstrap per our docs.

![Off-canvas navigation example]()

**Off-canvas**

Build a toggleable off-canvas navigation menu for use with Bootstrap.

### Tools

#### Bootlint

**[Bootlint](https://github.com/twbs/bootlint)** is the official Bootstrap HTML [linter](http://en.wikipedia.org/wiki/Lint_(software)) tool. It automatically checks for several common HTML mistakes in webpages that are using Bootstrap in a fairly "vanilla" way. Vanilla Bootstrap's components/widgets require their parts of the DOM to conform to certain structures. Bootlint checks that instances of Bootstrap components have correctly-structured HTML. Consider adding Bootlint to your Bootstrap web development toolchain so that none of the common mistakes slow down your project's development.

### Community

**Stay up to date on the development of Bootstrap and reach out to the community with these helpful resources.**

* Read and subscribe to [The Official Bootstrap Blog](http://blog.getbootstrap.com/).
* Chat with fellow Bootstrappers using IRC in the `irc.freenode.net` server, in the [##bootstrap channel](irc://irc.freenode.net/%23bootstrap).
* For help using Bootstrap, ask on [StackOverflow using the tag](https://stackoverflow.com/questions/tagged/twitter-bootstrap-3) `twitter-bootstrap-3`.
* Developers should use the keyword `bootstrap` on packages which modify or add to the functionality of Bootstrap when distributing through [npm](https://www.npmjs.com/browse/keyword/bootstrap) or similar delivery mechanisms for maximum discoverability.
* Find inspiring examples of people building with Bootstrap at the [Bootstrap Expo](http://expo.getbootstrap.com/).

You can also follow [@getbootstrap on Twitter](https://twitter.com/getbootstrap) for the latest gossip and awesome music videos.

### Disabling responsiveness

**Bootstrap automatically adapts your pages for various screen sizes. Here's how to disable this feature so your page works like [this non-responsive example](https://getbootstrap.com/docs/3.3/examples/non-responsive/).**

##### Steps to disable page responsiveness

1. Omit the viewport `<meta>` mentioned in [the CSS docs](https://getbootstrap.com/docs/3.3/css/#overview-mobile)
2. Override the `width` on the `.container` for each grid tier with a single `width, for example width: 970px !important;` Be sure that this comes after the default Bootstrap CSS. You can optionally avoid the `!important` with media queries or some selector-fu.
3. If using navbars, remove all navbar collapsing and expanding behavior.
4. For grid layouts, use `.col-xs-*` classes in addition to, or in place of, the medium/large ones. Don't worry, the extra-small device grid scales to all resolutions.

You'll still need Respond.js for IE8 (since our media queries are still there and need to be processed). This disables the "mobile site" aspects of Bootstrap.

#### Bootstrap template with responsiveness disabled

We've applied these steps to an example. Read its source code to see the specific changes implemented.

[View non-responsive example](https://getbootstrap.com/docs/3.3/examples/non-responsive/)

>**Migrating from v2.x to v3.x**
>
>>Looking to migrate from an older version of Bootstrap to v3.x? Check [out our migration guide](https://getbootstrap.com/docs/3.3/migration).

### Browser and device support

**Bootstrap is built to work best in the latest desktop and mobile browsers, meaning older browsers might display differently styled, though fully functional, renderings of certain components.**

#### Supported browsers

Specifically, we support the **latest versions** of the following browsers and platforms.

Alternative browsers which use the latest version of WebKit, Blink, or Gecko, whether directly or via the platform's web view API, are not explicitly supported. However, Bootstrap should (in most cases) display and function correctly in these browsers as well. More specific support information is provided below.

##### Mobile devices

Generally speaking, Bootstrap supports the latest versions of each major platform's default browsers. Note that proxy browsers (such as Opera Mini, Opera Mobile's Turbo mode, UC Browser Mini, Amazon Silk) are not supported.

| | Chrome | Firefox | Safari |
|------|------|------|------| 
| Android | Supported | Supported | N/A |
| iOS | Supported | Supported | Supported |

##### Desktop browsers

Similarly, the latest versions of most desktop browsers are supported.

| | Chrome | Firefox | Internet Explorer | Opera | Safari |
|------|------|------|------|------|------| 
| Mac | Supported | Supported | N/A | Supported | Supported |
| Windows | Supported | Supported | Supported | Supported | Not supported |

On Windows, **we support Internet Explorer 8-11**.

For Firefox, in addition to the latest normal stable release, we also support the latest [Extended Support Release (ESR)](https://www.mozilla.org/en-US/firefox/organizations/faq/) version of Firefox.

Unofficially, Bootstrap should look and behave well enough in Chromium and Chrome for Linux, Firefox for Linux, and Internet Explorer 7, as well as Microsoft Edge, though they are not officially supported.

For a list of some of the browser bugs that Bootstrap has to grapple with, see our [Wall of browser bugs](https://getbootstrap.com/docs/3.3/browser-bugs/).

#### Internet Explorer 8 and 9

Internet Explorer 8 and 9 are also supported, however, please be aware that some CSS3 properties and HTML5 elements are not fully supported by these browsers. In addition, **Internet Explorer 8 requires the use of [Respond.js](https://github.com/scottjehl/Respond) to enable media query support**.

| Feature | Internet Explorer 8 | Internet Explorer 9 |
|------|------|------|
| `border-radius` | Not supported | Supported |
| `box-shadow` | Not supported | Supported |
| `transform` | Not supported | Supported, with `-ms` prefix |
| `transition` | Not supported |
| `placeholder` | Not supported |

Visit [Can I use...](http://caniuse.com/) for details on browser support of CSS3 and HTML5 features.

#### Internet Explorer 8 and Respond.js

Beware of the following caveats when using Respond.js in your development and production environments for Internet Explorer 8.

##### Respond.js and cross-domain CSS

Using Respond.js with CSS hosted on a different (sub)domain (for example, on a CDN) requires some additional setup. [See the Respond.js docs](https://github.com/scottjehl/Respond/blob/master/README.md#cdnx-domain-setup) for details.

##### Respond.js and `file://`

Due to browser security rules, Respond.js doesn't work with pages viewed via the `file://` protocol (like when opening a local HTML file). To test responsive features in IE8, view your pages over HTTP(S). [See the Respond.js docs](https://github.com/scottjehl/Respond/blob/master/README.md#support--caveats) for details.

##### Respond.js and `@import`

Respond.js doesn't work with CSS that's referenced via `@import`. In particular, some Drupal configurations are known to use @import. [See the Respond.js docs](https://github.com/scottjehl/Respond/blob/master/README.md#support--caveats) for details.

#### Internet Explorer 8 and box-sizing

IE8 does not fully support `box-sizing: border-box;` when combined with `min-width`, `max-width`, `min-height`, or `max-height`. For that reason, as of v3.0.1, we no longer use `max-width` on `.containers`.

#### Internet Explorer 8 and @font-face

IE8 has some issues with `@font-face` when combined with `:before.` Bootstrap uses that combination with its Glyphicons. If a page is cached, and loaded without the mouse over the window (i.e. hit the refresh button or load something in an iframe) then the page gets rendered before the font loads. Hovering over the page (body) will show some of the icons and hovering over the remaining icons will show those as well. [See issue #13863](https://github.com/twbs/bootstrap/issues/13863) for details.

#### IE Compatibility modes

Bootstrap is not supported in the old Internet Explorer compatibility modes. To be sure you're using the latest rendering mode for IE, consider including the appropriate `<meta>` tag in your pages:

    ```html
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    ```

Confirm the document mode by opening the debugging tools: press **[F12]** and check the "Document Mode".

This tag is included in all of Bootstrap's documentation and examples to ensure the best rendering possible in each supported version of Internet Explorer.

See [this StackOverflow question](https://stackoverflow.com/questions/6771258/whats-the-difference-if-meta-http-equiv-x-ua-compatible-content-ie-edge) for more information.

#### Internet Explorer 10 in Windows 8 and Windows Phone 8

Internet Explorer 10 doesn't differentiate **device width** from **viewport width**, and thus doesn't properly apply the media queries in Bootstrap's CSS. Normally you'd just add a quick snippet of CSS to fix this:

    ```css
    @-ms-viewport       { width: device-width; }
    ```

However, this doesn't work for devices running Windows Phone 8 versions older than [Update 3 (a.k.a. GDR3)](http://blogs.windows.com/windows_phone/b/wpdev/archive/2013/10/14/introducing-windows-phone-preview-for-developers.aspx), as it causes such devices to show a mostly desktop view instead of narrow "phone" view. To address this, you'll need to **include the following CSS and JavaScript to work around the bug**.

    ```css
    @-ms-viewport       { width: device-width; }
    @-o-viewport        { width: device-width; }
    @viewport           { width: device-width; }
    ```

    ```javascript
    // right 2014-2015 Twitter, Inc.
    // Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
    if (navigator.userAgent.match(/IEMobile\/10\.0/)) {
      var msViewportStyle = document.createElement('style')
      msViewportStyle.appendChild(
        document.createTextNode(
          '@-ms-viewport{width:auto!important}'
        )
      )
      document.querySelector('head').appendChild(msViewportStyle)
    }
    ```

For more information and usage guidelines, read [Windows Phone 8 and Device-Width](http://timkadlec.com/2013/01/windows-phone-8-and-device-width/).

As a heads up, we include this in all of Bootstrap's documentation and examples as a demonstration.

#### Safari percent rounding

The rendering engine of versions of Safari prior to v7.1 for OS X and Safari for iOS v8.0 had some trouble with the number of decimal places used in our `.col-*-1` grid classes. So if you had 12 individual grid columns, you'd notice that they came up short compared to other rows of columns. Besides upgrading Safari/iOS, you have some options for workarounds:

* Add `.pull-right` to your last grid column to get the hard-right alignment
* Tweak your percentages manually to get the perfect rounding for Safari (more difficult than the first option)

#### Modals, navbars, and virtual keyboards

##### Overflow and scrolling

Support for `overflow: hidden` on the `<body>` element is quite limited in iOS and Android. To that end, when you scroll past the top or bottom of a modal in either of those devices' browsers, the `<body>` content will begin to scroll. See [Crome bug #175502](https://bugs.chromium.org/p/chromium/issues/detail?id=175502) (fixed in Chrome v40) and [WebKit bug #153852](https://bugs.webkit.org/show_bug.cgi?id=153852).

##### iOS text fields and scrolling

As of iOS 9.3, while a modal is open, if the initial touch of a scroll gesture is within the boundary of a textual `<input>` or a `<textarea>`, the `<body>` content underneath the modal will be scrolled instead of the modal itself. See [WebKit bug #153856](https://bugs.webkit.org/show_bug.cgi?id=153856).

#### Virtual keyboards

Also, note that if you're using a fixed navbar or using inputs within a modal, iOS has a rendering bug that doesn't update the position of fixed elements when the virtual keyboard is triggered. A few workarounds for this include transforming your elements to `position: absolute` or invoking a timer on focus to try to correct the positioning manually. This is not handled by Bootstrap, so it is up to you to decide which solution is best for your application.

##### Navbar Dropdowns

The `.dropdown-backdrop` element isn't used on iOS in the nav because of the complexity of z-indexing. Thus, to close dropdowns in navbars, you must directly click the dropdown element (or [any other element which will fire a click event in iOS](https://developer.mozilla.org/en-US/docs/Web/Events/click#Safari_Mobile)).

#### Browser zooming

Page zooming inevitably presents rendering artifacts in some components, both in Bootstrap and the rest of the web. Depending on the issue, we may be able to fix it (search first and then open an issue if need be). However, we tend to ignore these as they often have no direct solution other than hacky workarounds.

#### Sticky `:hover`/`:focus` on mobile

Even though real hovering isn't possible on most touchscreens, most mobile browsers emulate hovering support and make `:hover` "sticky". In other words, `:hover` styles start applying after tapping an element and only stop applying after the user taps some other element. This can cause Bootstrap's `:hover` states to become undesirably "stuck" on such browsers. Some mobile browsers also make `:focus` similarly sticky. There is currently no simple workaround for these issues other than removing such styles entirely.

#### Printing

Even in some modern browsers, printing can be quirky.

In particular, as of Chrome v32 and regardless of margin settings, Chrome uses a viewport width significantly narrower than the physical paper size when resolving media queries while printing a webpage. This can result in Bootstrap's extra-small grid being unexpectedly activated when printing. [See issue #12078](https://github.com/twbs/bootstrap/issues/12078) and [Chrome bug #273306](https://bugs.chromium.org/p/chromium/issues/detail?id=273306) for some details. Suggested workarounds:

* Embrace the extra-small grid and make sure your page looks acceptable under it.
* Customize the values of the `@screen-*` Less variables so that your printer paper is considered larger than extra-small.
* Add custom media queries to change the grid size breakpoints for print media only.

Also, as of Safari v8.0, fixed-width `.containers` can cause Safari to use an unusually small font size when printing. See [#14868](https://github.com/twbs/bootstrap/issues/14868) and [WebKit bug #138192](https://bugs.webkit.org/show_bug.cgi?id=138192) for more details. One potential workaround for this is adding the following CSS:

    ```css
    @media print {
      .container {
        width: auto;
      }
    }
    ```

#### Android stock browser

Out of the box, Android 4.1 (and even some newer releases apparently) ship with the Browser app as the default web browser of choice (as opposed to Chrome). Unfortunately, the Browser app has lots of bugs and inconsistencies with CSS in general.

##### Select menus

On `<select>` elements, the Android stock browser will not display the side controls if there is a `border-radius` and/or `border` applied. (See `[this StackOverflow question](https://stackoverflow.com/questions/14744437/html-select-box-not-showing-drop-down-arrow-on-android-version-4-0-when-set-with) for details.) Use the snippet of code below to remove the offending CSS and render the `<select>` as an unstyled element on the Android stock browser. The user agent sniffing avoids interference with Chrome, Safari, and Mozilla browsers.


    ```html
    <script>
    $(function () {
      var nua = navigator.userAgent
      var isAndroid = (nua.indexOf('Mozilla/5.0') > -1 && nua.indexOf('Android ') > -1 && nua.indexOf('AppleWebKit') > -1 && nua.indexOf('Chrome') === -1)
      if (isAndroid) {
        $('select.form-control').removeClass('form-control').css('width', '100%')
      }
    })
    </script>
    ```

Want to see an example? [Check out this JS Bin demo](http://jsbin.com/kuvoz/1).

#### Validators

In order to provide the best possible experience to old and buggy browsers, Bootstrap uses [CSS browser hacks](http://browserhacks.com/) in several places to target special CSS to certain browser versions in order to work around bugs in the browsers themselves. These hacks understandably cause CSS validators to complain that they are invalid. In a couple places, we also use bleeding-edge CSS features that aren't yet fully standardized, but these are used purely for progressive enhancement.

These validation warnings don't matter in practice since the non-hacky portion of our CSS does fully validate and the hacky portions don't interfere with the proper functioning of the non-hacky portion, hence why we deliberately ignore these particular warnings.

Our HTML docs likewise have some trivial and inconsequential HTML validation warnings due to our inclusion of a workaround for [a certain Firefox bug](https://bugzilla.mozilla.org/show_bug.cgi?id=654072).

### Third party support

**While we don't officially support any third party plugins or add-ons, we do offer some useful advice to help avoid potential issues in your projects.**

#### Box-sizing

Some third party software, including Google Maps and Google Custom Search Engine, conflict with Bootstrap due to `* { box-sizing: border-box; }`, a rule which makes it so `padding` does not affect the final computed width of an element. Learn more about [box model and sizing at CSS Tricks](https://css-tricks.com/box-sizing/).

Depending on the context, you may override as-needed (Option 1) or reset the box-sizing for entire regions (Option 2).

    ```CSS
    /* Box-sizing resets
     *
     * Reset individual elements or override regions to avoid conflicts due to
     * global box model settings of Bootstrap. Two options, individual overrides and
     * region resets, are available as plain CSS and uncompiled Less formats.
     */
    /* Option 1A: Override a single element's box model via CSS */
    .element {
      -webkit-box-sizing: content-box;
         -moz-box-sizing: content-box;
              box-sizing: content-box;
    }
    /* Option 1B: Override a single element's box model by using a Bootstrap Less mixin */
    .element {
      .box-sizing(content-box);
    }
    /* Option 2A: Reset an entire region via CSS */
    .reset-box-sizing,
    .reset-box-sizing *,
    .reset-box-sizing *:before,
    .reset-box-sizing *:after {
      -webkit-box-sizing: content-box;
         -moz-box-sizing: content-box;
              box-sizing: content-box;
    }
    /* Option 2B: Reset an entire region with a custom Less mixin */
    .reset-box-sizing {
      &,
      *,
      *:before,
      *:after {
        .box-sizing(content-box);
      }
    }
    .element {
      .reset-box-sizing();
    }
    ```

### Accessibility

**Bootstrap follows common web standards and—with minimal extra effort—can be used to create sites that are accessible to those using AT.**

#### Skip navigation

If your navigation contains many links and comes before the main content in the DOM, add a `Skip to main content` link before the navigation (for a simple explanation, see this [A11Y Project article on skip navigation links](http://a11yproject.com/posts/skip-nav-links)). Using the `.sr-only` class will visually hide the skip link, and the `.sr-only-focusable` class will ensure that the link becomes visible once focused (for sighted keyboard users).

> Due to long-standing shortcomings/bugs in Chrome (see [issue 262171 in the Chromium bug tracker](https://code.google.com/p/chromium/issues/detail?id=262171)) and Internet Explorer (see this article on [in-page links and focus order](http://accessibleculture.org/articles/2010/05/in-page-links/)), you will need to make sure that the target of your skip link is at least programmatically focusable by adding `tabindex="-1"`.
> 
> In addition, you may want to explicitly suppress a visible focus indication on the target (particularly as Chrome currently also sets focus on elements with `tabindex="-1"` when they are clicked with the mouse) with `#content:focus { outline: none; }`.
> 
> Note that this bug will also affect any other in-page links your site may be using, rendering them useless for keyboard users. You may consider adding a similar stop-gap fix to all other named anchors / fragment identifiers that act as link targets.

    ```html
    <body>
      <a href="#content" class="sr-only sr-only-focusable">Skip to main content</a>
      ...
      <div class="container" id="content" tabindex="-1">
        <!-- The main page content -->
      </div>
    </body>
    ```

#### Nested headings

When nesting headings (`<h1>` - `<h6>`), your primary document header should be an `<h1>`. Subsequent headings should make logical use of `<h2>` - `<h6>` such that screen readers can construct a table of contents for your pages.

Learn more at [HTML CodeSniffer](http://squizlabs.github.io/HTML_CodeSniffer/Standards/Section508/) and [Penn State's AccessAbility](http://accessibility.psu.edu/headings).

#### Color contrast

Currently, some of the default color combinations available in Bootstrap (such as the various styled button classes, some of the code highlighting colors used for [basic code blocks](https://getbootstrap.com/docs/3.3/css/#code-block), the `.bg-primary` [contextual background](https://getbootstrap.com/docs/3.3/css/#helper-classes-backgrounds) helper class, and the default link color when used on a white background) have a low contrast ratio (below the [recommended ratio of 4.5:1](http://www.w3.org/TR/WCAG20/#visual-audio-contrast-contrast)). This can cause problems to users with low vision or who are color blind. These default colors may need to be modified to increase their contrast and legibility.

#### Additional resources

* ["HTML Codesniffer" bookmarklet for identifying accessibility issues](https://github.com/squizlabs/HTML_CodeSniffer)
* [Chrome's Accessibility Developer Tools extension](https://chrome.google.com/webstore/detail/accessibility-developer-t/fpkknkljclfencbdbgkenhalefipecmb?hl=en)
* [Colour Contrast Analyser](http://www.paciellogroup.com/resources/contrastanalyser/)
* [The A11Y Project](http://a11yproject.com/)
* [MDN accessibility documentation](https://developer.mozilla.org/en-US/docs/Accessibility)

### License FAQs

**Bootstrap is released under the MIT license and is right 2016 Twitter. Boiled down to smaller chunks, it can be described with the following conditions.**

#### It requires you to:

* Keep the license and right notice included in Bootstrap's CSS and JavaScript files when you use them in your works

#### It permits you to:

* Freely download and use Bootstrap, in whole or in part, for personal, private, company internal, or commercial purposes
* Use Bootstrap in packages or distributions that you create
* Modify the source code
* Grant a sublicense to modify and distribute Bootstrap to third parties not included in the license

#### It forbids you to:

* Hold the authors and license owners liable for damages as Bootstrap is provided without warranty
* Hold the creators or right holders of Bootstrap liable
* Redistribute any piece of Bootstrap without proper attribution
* Use any marks owned by Twitter in any way that might state or imply that Twitter endorses your distribution
* Use any marks owned by Twitter in any way that might state or imply that you created the Twitter software in question

#### It does not require you to:

* Include the source of Bootstrap itself, or of any modifications you may have made to it, in any redistribution you may assemble that includes it
* Submit changes that you make to Bootstrap back to the Bootstrap project (though such feedback is encouraged)

The full Bootstrap license is located [in the project repository](https://github.com/twbs/bootstrap/blob/master/LICENSE) for more information.

### Translations

**Community members have translated Bootstrap's documentation into various languages. None are officially supported and they may not always be up to date.**

* [Bootstrap 中文文档 (Chinese)](http://v3.bootcss.com/)
* [Bootstrap 3 中文手冊 (Chinese (Traditional))](https://kkbruce.tw/bs3/)
* [Bootstrap på Dansk (Danish)](http://getbootstrap.dk/)
* [Bootstrap en Français (French)](http://www.oneskyapp.com/fr/docs/bootstrap/getting-started/)
* [Bootstrap auf Deutsch (German)](http://holdirbootstrap.de/)
* [Bootstrap in Italiano (Italian)](http://www.hackerstribe.com/guide/IT-bootstrap-3.1.1/)
* [Bootstrap 한국어 (Korean)](http://bootstrapk.com/)
* [Bootstrap em Português do Brasil (Brazilian Portuguese)](http://bootstrapbrasil.github.io/)
* [Bootstrap по-русски (Russian)](http://www.oneskyapp.com/ru/docs/bootstrap/)
* [Bootstrap en Español (Spanish)](http://www.oneskyapp.com/es/docs/bootstrap/)
* [Türkçe Bootstrap (Turkish)](http://www.trbootstrap.com/)
* [Bootstrap українською (Ukrainian)](http://twbs.docs.org.ua/)
* [Bootstrap bằng tiếng Việt (Vietnamese)](http://getbootstrap.com.vn/)

**We don't help organize or host translations, we just link to them.**

Finished a new or better translation? Open a pull request to add it to our list.

-------------------------------------------------------------------------------

## CSS

**Global CSS settings, fundamental HTML elements styled and enhanced with extensible classes, and an advanced grid system.**

### Overview

Get the lowdown on the key pieces of Bootstrap's infrastructure, including our approach to better, faster, stronger web development.

#### HTML5 doctype

Bootstrap makes use of certain HTML elements and CSS properties that require the use of the HTML5 doctype. Include it at the beginning of all your projects.

    ```html
    <!DOCTYPE html>
    <html lang="en">
      ...
    </html>
    ```

#### Mobile first

With Bootstrap 2, we added optional mobile friendly styles for key aspects of the framework. With Bootstrap 3, we've rewritten the project to be mobile friendly from the start. Instead of adding on optional mobile styles, they're baked right into the core. In fact, **Bootstrap is mobile first. Mobile first** styles can be found throughout the entire library instead of in separate files.

To ensure proper rendering and touch zooming, **add the viewport meta tag** to your `<head>`.

    ```html
    <meta name="viewport" content="width=device-width, initial-scale=1">
    ```

You can disable zooming capabilities on mobile devices by adding user-scalable=no to the viewport meta tag. This disables zooming, meaning users are only able to scroll, and results in your site feeling a bit more like a native application. Overall, we don't recommend this on every site, so use caution!

    ```html
    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no">
    ```

#### Typography and links

Bootstrap sets basic global display, typography, and link styles. Specifically, we:

* Set `background-color: #fff;` on the body
* Use the `@font-family-base`, `@font-size-base`, and `@line-height-base` attributes as our typographic base
* Set the global link color via `@link-color` and apply link underlines only on `:hover`

These styles can be found within `scaffolding.less`.

#### Normalize.css

For improved cross-browser rendering, we use [Normalize.css](http://necolas.github.io/normalize.css/), a project by [Nicolas Gallagher](https://twitter.com/necolas) and [Jonathan Neal](https://twitter.com/jon_neal).

#### Containers

Bootstrap requires a containing element to wrap site contents and house our grid system. You may choose one of two containers to use in your projects. Note that, due to padding and more, neither container is nestable.

Use `.container` for a responsive fixed width container.


    ```html
    <div class="container">
      ...
    </div>
    ```

Use `.container-fluid` for a full width container, spanning the entire width of your viewport.


    ```html
    <div class="container-fluid">
      ...
    </div>
    ```

### Grid system

**Bootstrap includes a responsive, mobile first fluid grid system that appropriately scales up to 12 columns as the device or viewport size increases. It includes [predefined classes](https://getbootstrap.com/docs/3.3/css/#grid-example-basic) for easy layout options, as well as powerful [mixins for generating more semantic layouts](https://getbootstrap.com/docs/3.3/css/#grid-less).**

#### Introduction

Grid systems are used for creating page layouts through a series of rows and columns that house your content. Here's how the Bootstrap grid system works:

* Rows must be placed within a `.container` (fixed-width) or `.container-fluid` (full-width) for proper alignment and padding.
* Use rows to create horizontal groups of columns.
* Content should be placed within columns, and only columns may be immediate children of rows.
* Predefined grid classes like `.row` and `.col-xs-4` are available for quickly making grid layouts. Less mixins can also be used for more semantic layouts.
* Columns create gutters (gaps between column content) via `padding`. That padding is offset in rows for the first and last column via negative margin on `.rows`.
* The negative margin is why the examples below are outdented. It's so that content within grid columns is lined up with non-grid content.
* Grid columns are created by specifying the number of twelve available columns you wish to span. For example, three equal columns would use three `.col-xs-4`.
* If more than 12 columns are placed within a single row, each group of extra columns will, as one unit, wrap onto a new line.
* Grid classes apply to devices with screen widths greater than or equal to the breakpoint sizes, and override grid classes targeted at smaller devices. Therefore, e.g. applying any `.col-md-*` class to an element will not only affect its styling on medium devices but also on large devices if a `.col-lg-*` class is not present.

Look to the examples for applying these principles to your code.

#### Media queries

We use the following media queries in our Less files to create the key breakpoints in our grid system.

    ```css
    /* Extra small devices (phones, less than 768px) */
    /* No media query since this is the default in Bootstrap */
    /* Small devices (tablets, 768px and up) */
    @media (min-width: @screen-sm-min) { ... }
    /* Medium devices (desktops, 992px and up) */
    @media (min-width: @screen-md-min) { ... }
    /* Large devices (large desktops, 1200px and up) */
    @media (min-width: @screen-lg-min) { ... }
    ```

We occasionally expand on these media queries to include a max-width to limit CSS to a narrower set of devices.

    ```css
    @media (max-width: @screen-xs-max) { ... }
    @media (min-width: @screen-sm-min) and (max-width: @screen-sm-max) { ... }
    @media (min-width: @screen-md-min) and (max-width: @screen-md-max) { ... }
    @media (min-width: @screen-lg-min) { ... }
    ```

#### Grid options

See how aspects of the Bootstrap grid system work across multiple devices with a handy table.

| | Extra small devices Phones (<768px) | Small devices Tablets (≥768px) | Medium devices Desktops (≥992px) | Large devices Desktops (≥1200px) |
|-------|------|------|------|------|
| Grid behavior | Horizontal at all times | Collapsed to start, horizontal above breakpoints |
| Container width | None (auto) | 750px | 970px | 1170px |
| Class prefix | col-xs- | .col-sm- | col-md- | .col-lg- |
| # of columns | 12 |
| Column width | Auto | ~62px | ~81px | ~97px |
| Gutter width | 30px (15px on each side of a column) |
| Nestable | Yes |
| Offsets | Yes |
| Column ordering | Yes |

#### Example: Stacked-to-horizontal

Using a single set of .col-md-* grid classes, you can create a basic grid system that starts out stacked on mobile devices and tablet devices (the extra small to small range) before becoming horizontal on desktop (medium) devices. Place grid columns in any `.row`.

| .col-md-1 | .col-md-1 | .col-md-1 | .col-md-1 | .col-md-1 | .col-md-1 | .col-md-1 | .col-md-1 | .col-md-1 | .col-md-1 | .col-md-1 | .col-md-1 |
| .col-md-8 | .col-md-4 |
| .col-md-4 | .col-md-4 | .col-md-4 |
| .col-md-6 | .col-md-6 |


    ```html
    <div class="row">
      <div class="col-md-1">.col-md-1</div>
      <div class="col-md-1">.col-md-1</div>
      <div class="col-md-1">.col-md-1</div>
      <div class="col-md-1">.col-md-1</div>
      <div class="col-md-1">.col-md-1</div>
      <div class="col-md-1">.col-md-1</div>
      <div class="col-md-1">.col-md-1</div>
      <div class="col-md-1">.col-md-1</div>
      <div class="col-md-1">.col-md-1</div>
      <div class="col-md-1">.col-md-1</div>
      <div class="col-md-1">.col-md-1</div>
      <div class="col-md-1">.col-md-1</div>
    </div>
    <div class="row">
      <div class="col-md-8">.col-md-8</div>
      <div class="col-md-4">.col-md-4</div>
    </div>
    <div class="row">
      <div class="col-md-4">.col-md-4</div>
      <div class="col-md-4">.col-md-4</div>
      <div class="col-md-4">.col-md-4</div>
    </div>
    <div class="row">
      <div class="col-md-6">.col-md-6</div>
      <div class="col-md-6">.col-md-6</div>
    </div>
    ```

#### Example: Fluid container

Turn any fixed-width grid layout into a full-width layout by changing your outermost `.container` to `.container-fluid`.

    ```html
    <div class="container-fluid">
      <div class="row">
        ...
      </div>
    </div>
    ```

#### Example: Mobile and desktop

Don't want your columns to simply stack in smaller devices? Use the extra small and medium device grid classes by adding `.col-xs-* .col-md-*` to your columns. See the example below for a better idea of how it all works.

| .col-xs-12 .col-md-8 | .col-xs-6 .col-md-4 |
| .col-xs-6 .col-md-4 | .col-xs-6 .col-md-4 | .col-xs-6 .col-md-4 |
| .col-xs-6 | .col-xs-6 |

    ```html
    <!-- Stack the columns on mobile by making one full-width and the other half-width -->
    <div class="row">
      <div class="col-xs-12 col-md-8">.col-xs-12 .col-md-8</div>
      <div class="col-xs-6 col-md-4">.col-xs-6 .col-md-4</div>
    </div>
    <!-- Columns start at 50% wide on mobile and bump up to 33.3% wide on desktop -->
    <div class="row">
      <div class="col-xs-6 col-md-4">.col-xs-6 .col-md-4</div>
      <div class="col-xs-6 col-md-4">.col-xs-6 .col-md-4</div>
      <div class="col-xs-6 col-md-4">.col-xs-6 .col-md-4</div>
    </div>
    <!-- Columns are always 50% wide, on mobile and desktop -->
    <div class="row">
      <div class="col-xs-6">.col-xs-6</div>
      <div class="col-xs-6">.col-xs-6</div>
    </div>
    ```

#### Example: Mobile, tablet, desktop

Build on the previous example by creating even more dynamic and powerful layouts with tablet `.col-sm-*` classes.

| .col-xs-12 .col-sm-6 .col-md-8 | .col-xs-6 .col-md-4 |
| .col-xs-6 .col-sm-4 | .col-xs-6 .col-sm-4 | .col-xs-6 .col-sm-4 |

    ```html
    <div class="row">
      <div class="col-xs-12 col-sm-6 col-md-8">.col-xs-12 .col-sm-6 .col-md-8</div>
      <div class="col-xs-6 col-md-4">.col-xs-6 .col-md-4</div>
    </div>
    <div class="row">
      <div class="col-xs-6 col-sm-4">.col-xs-6 .col-sm-4</div>
      <div class="col-xs-6 col-sm-4">.col-xs-6 .col-sm-4</div>
      <!-- Optional: clear the XS cols if their content doesn't match in height -->
      <div class="clearfix visible-xs-block"></div>
      <div class="col-xs-6 col-sm-4">.col-xs-6 .col-sm-4</div>
    </div>
    ```

#### Example: Column wrapping

If more than 12 columns are placed within a single row, each group of extra columns will, as one unit, wrap onto a new line.
| .col-xs-9 |

| .col-xs-4 Since 9 + 4 = 13 > 12, this 4-column-wide div gets wrapped onto a new line as one contiguous unit. | .col-xs-6 Subsequent columns continue along the new line. |

    ```html
    <div class="row">
      <div class="col-xs-9">.col-xs-9</div>
      <div class="col-xs-4">.col-xs-4<br>Since 9 + 4 = 13 &gt; 12, this 4-column-wide div gets wrapped onto a new line as one contiguous unit.</div>
      <div class="col-xs-6">.col-xs-6<br>Subsequent columns continue along the new line.</div>
    </div>
    ```

#### Responsive column resets

With the four tiers of grids available you're bound to run into issues where, at certain breakpoints, your columns don't clear quite right as one is taller than the other. To fix that, use a combination of a `.clearfix` and our [responsive utility classes](https://getbootstrap.com/docs/3.3/css/#responsive-utilities).

| .col-xs-6 .col-sm-3 Resize your viewport or check it out on your phone for an example. | .col-xs-6 .col-sm-3 | .col-xs-6 .col-sm-3 | .col-xs-6 .col-sm-3 |

    ```html
    <div class="row">
      <div class="col-xs-6 col-sm-3">.col-xs-6 .col-sm-3</div>
      <div class="col-xs-6 col-sm-3">.col-xs-6 .col-sm-3</div>
      <!-- Add the extra clearfix for only the required viewport -->
      <div class="clearfix visible-xs-block"></div>
      <div class="col-xs-6 col-sm-3">.col-xs-6 .col-sm-3</div>
      <div class="col-xs-6 col-sm-3">.col-xs-6 .col-sm-3</div>
    </div>
    ```

In addition to column clearing at responsive breakpoints, you may need to **reset offsets, pushes, or pulls**. See this in action in [the grid example](https://getbootstrap.com/docs/3.3/examples/grid/).

    ```html
    <div class="row">
      <div class="col-sm-5 col-md-6">.col-sm-5 .col-md-6</div>
      <div class="col-sm-5 col-sm-offset-2 col-md-6 col-md-offset-0">.col-sm-5 .col-sm-offset-2 .col-md-6 .col-md-offset-0</div>
    </div>

    <div class="row">
      <div class="col-sm-6 col-md-5 col-lg-6">.col-sm-6 .col-md-5 .col-lg-6</div>
      <div class="col-sm-6 col-md-5 col-md-offset-2 col-lg-6 col-lg-offset-0">.col-sm-6 .col-md-5 .col-md-offset-2 .col-lg-6 .col-lg-offset-0</div>
    </div>
    ```

#### Offsetting columns

Move columns to the right using `.col-md-offset-*` classes. These classes increase the left margin of a column by * columns. For example, `.col-md-offset-4` moves `.col-md-4` over four columns.

| .col-md-4 |  | .col-md-4 .col-md-offset-4 |
| | .col-md-3 .col-md-offset-3 | | .col-md-3 .col-md-offset-3 | 
| | .col-md-6 .col-md-offset-3 | |

    ```html
    <div class="row">
      <div class="col-md-4">.col-md-4</div>
      <div class="col-md-4 col-md-offset-4">.col-md-4 .col-md-offset-4</div>
    </div>
    <div class="row">
      <div class="col-md-3 col-md-offset-3">.col-md-3 .col-md-offset-3</div>
      <div class="col-md-3 col-md-offset-3">.col-md-3 .col-md-offset-3</div>
    </div>
    <div class="row">
      <div class="col-md-6 col-md-offset-3">.col-md-6 .col-md-offset-3</div>
    </div>
    ```

You can also override offsets from lower grid tiers with `.col-*-offset-0` classes.

    ```html
    <div class="row">
      <div class="col-xs-6 col-sm-4">
      </div>
      <div class="col-xs-6 col-sm-4">
      </div>
      <div class="col-xs-6 col-xs-offset-3 col-sm-4 col-sm-offset-0">
      </div>
    </div>
    ```

#### Nesting column

To nest your content with the default grid, add a new `.row` and set of `.col-sm-*` columns within an existing `.col-sm-*` column. Nested rows should include a set of columns that add up to 12 or fewer (it is not required that you use all 12 available columns).

| Level 1: .col-sm-9 |
| Level 2: .col-xs-8 .col-sm-6 | Level 2: .col-xs-4 .col-sm-6 |

    ```html
    <div class="row">
      <div class="col-sm-9">
        Level 1: .col-sm-9
        <div class="row">
          <div class="col-xs-8 col-sm-6">
            Level 2: .col-xs-8 .col-sm-6
          </div>
          <div class="col-xs-4 col-sm-6">
            Level 2: .col-xs-4 .col-sm-6
          </div>
        </div>
      </div>
    </div>
    ```

#### Column ordering

Easily change the order of our built-in grid columns with `.col-md-push-*` and `.col-md-pull-*` modifier classes.

| .col-md-9 .col-md-push-3 | .col-md-3 .col-md-pull-9 |

    ```html
    <div class="row">
      <div class="col-md-9 col-md-push-3">.col-md-9 .col-md-push-3</div>
      <div class="col-md-3 col-md-pull-9">.col-md-3 .col-md-pull-9</div>
    </div>
    ```

#### Less mixins and variables

In addition to prebuilt grid classes for fast layouts, Bootstrap includes Less variables and mixins for quickly generating your own simple, semantic layouts.

##### Variables

Variables determine the number of columns, the gutter width, and the media query point at which to begin floating columns. We use these to generate the predefined grid classes documented above, as well as for the custom mixins listed below.

    ```css
    @grid-columns:              12;
    @grid-gutter-width:         30px;
    @grid-float-breakpoint:     768px;
    ```

##### Mixins

Mixins are used in conjunction with the grid variables to generate semantic CSS for individual grid columns.

    ```css
    // Creates a wrapper for a series of columns
    .make-row(@gutter: @grid-gutter-width) {
      // Then clear the floated columns
      .clearfix();
      @media (min-width: @screen-sm-min) {
        margin-left:  (@gutter / -2);
        margin-right: (@gutter / -2);
      }
      // Negative margin nested rows out to align the content of columns
      .row {
        margin-left:  (@gutter / -2);
        margin-right: (@gutter / -2);
      }
    }
    // Generate the extra small columns
    .make-xs-column(@columns; @gutter: @grid-gutter-width) {
      position: relative;
      // Prevent columns from collapsing when empty
      min-height: 1px;
      // Inner gutter via padding
      padding-left:  (@gutter / 2);
      padding-right: (@gutter / 2);
      // Calculate width based on number of columns available
      @media (min-width: @grid-float-breakpoint) {
        float: left;
        width: percentage((@columns / @grid-columns));
      }
    }
    // Generate the small columns
    .make-sm-column(@columns; @gutter: @grid-gutter-width) {
      position: relative;
      // Prevent columns from collapsing when empty
      min-height: 1px;
      // Inner gutter via padding
      padding-left:  (@gutter / 2);
      padding-right: (@gutter / 2);
      // Calculate width based on number of columns available
      @media (min-width: @screen-sm-min) {
        float: left;
        width: percentage((@columns / @grid-columns));
      }
    }
    // Generate the small column offsets
    .make-sm-column-offset(@columns) {
      @media (min-width: @screen-sm-min) {
        margin-left: percentage((@columns / @grid-columns));
      }
    }
    .make-sm-column-push(@columns) {
      @media (min-width: @screen-sm-min) {
        left: percentage((@columns / @grid-columns));
      }
    }
    .make-sm-column-pull(@columns) {
      @media (min-width: @screen-sm-min) {
        right: percentage((@columns / @grid-columns));
      }
    }
    // Generate the medium columns
    .make-md-column(@columns; @gutter: @grid-gutter-width) {
      position: relative;
      // Prevent columns from collapsing when empty
      min-height: 1px;
      // Inner gutter via padding
      padding-left:  (@gutter / 2);
      padding-right: (@gutter / 2);
      // Calculate width based on number of columns available
      @media (min-width: @screen-md-min) {
        float: left;
        width: percentage((@columns / @grid-columns));
      }
    }
    // Generate the medium column offsets
    .make-md-column-offset(@columns) {
      @media (min-width: @screen-md-min) {
        margin-left: percentage((@columns / @grid-columns));
      }
    }
    .make-md-column-push(@columns) {
      @media (min-width: @screen-md-min) {
        left: percentage((@columns / @grid-columns));
      }
    }
    .make-md-column-pull(@columns) {
      @media (min-width: @screen-md-min) {
        right: percentage((@columns / @grid-columns));
      }
    }
    // Generate the large columns
    .make-lg-column(@columns; @gutter: @grid-gutter-width) {
      position: relative;
      // Prevent columns from collapsing when empty
      min-height: 1px;
      // Inner gutter via padding
      padding-left:  (@gutter / 2);
      padding-right: (@gutter / 2);
      // Calculate width based on number of columns available
      @media (min-width: @screen-lg-min) {
        float: left;
        width: percentage((@columns / @grid-columns));
      }
    }
    // Generate the large column offsets
    .make-lg-column-offset(@columns) {
      @media (min-width: @screen-lg-min) {
        margin-left: percentage((@columns / @grid-columns));
      }
    }
    .make-lg-column-push(@columns) {
      @media (min-width: @screen-lg-min) {
        left: percentage((@columns / @grid-columns));
      }
    }
    .make-lg-column-pull(@columns) {
      @media (min-width: @screen-lg-min) {
        right: percentage((@columns / @grid-columns));
      }
    }
    ```

##### Example usage

You can modify the variables to your own custom values, or just use the mixins with their default values. Here's an example of using the default settings to create a two-column layout with a gap between.

    ```css
    .wrapper {
      .make-row();
    }
    .content-main {
      .make-lg-column(8);
    }
    .content-secondary {
      .make-lg-column(3);
      .make-lg-column-offset(1);
    }
    ```

    ```html
    <div class="wrapper">
      <div class="content-main">...</div>
      <div class="content-secondary">...</div>
    </div>
    ```

### Typography
#### Headings

All HTML headings, `<h1>` through `<h6>`, are available. `.h1` through `.h6` classes are also available, for when you want to match the font styling of a heading but still want your text to be displayed inline.

    Example
    # h1. Bootstrap heading
    	*Semibold 36px*
    ## h2. Bootstrap heading
    	*Semibold 30px*
    ### h3. Bootstrap heading
    	*Semibold 24px*
    #### h4. Bootstrap heading
    	*Semibold 18px*
    ##### h5. Bootstrap heading
    	*Semibold 14px*
    ###### h6. Bootstrap heading
    	*Semibold 12px*

```html
<h1>h1. Bootstrap heading</h1>
<h2>h2. Bootstrap heading</h2>
<h3>h3. Bootstrap heading</h3>
<h4>h4. Bootstrap heading</h4>
<h5>h5. Bootstrap heading</h5>
<h6>h6. Bootstrap heading</h6>
```

Create lighter, secondary text in any heading with a generic `<small>` tag or the `.small` class.

    Example
    # h1. Bootstrap heading Secondary text
    ## h2. Bootstrap heading Secondary text
    ### h3. Bootstrap heading Secondary text
    #### h4. Bootstrap heading Secondary text
    ##### h5. Bootstrap heading Secondary text
    ######h6. Bootstrap heading Secondary text

    ```html
    <h1>h1. Bootstrap heading <small>Secondary text</small></h1>
    <h2>h2. Bootstrap heading <small>Secondary text</small></h2>
    <h3>h3. Bootstrap heading <small>Secondary text</small></h3>
    <h4>h4. Bootstrap heading <small>Secondary text</small></h4>
    <h5>h5. Bootstrap heading <small>Secondary text</small></h5>
    <h6>h6. Bootstrap heading <small>Secondary text</small></h6>
    ```

#### Body 

Bootstrap's global default `font-size` is 14px, with a `line-height` of 1.428. This is applied to the `<body>` and all paragraphs. In addition, `<p>` (paragraphs) receive a bottom margin of half their computed line-height (10px by default).

    Example
    Nullam quis risus eget urna mollis ornare vel eu leo. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Nullam id dolor id nibh ultricies vehicula.

    Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec ullamcorper nulla non metus auctor fringilla. Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem nec elit. Donec ullamcorper nulla non metus auctor fringilla.

    Maecenas sed diam eget risus varius blandit sit amet non magna. Donec id elit non mi porta gravida at eget metus. Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem nec elit.
   

    Example
    <p>...</p>
    ```

##### Lead body 

Make a paragraph stand out by adding `.lead`.

    Example
    Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor. Duis mollis, est non commodo luctus.

    ```html
    <p class="lead">...</p>
    ```

##### Built with Less

The typographic scale is based on two Less variables in **variables.less**: `@font-size-base` and `@line-height`-base. The first is the base font-size used throughout and the second is the base line-height. We use those variables and some simple math to create the margins, paddings, and line-heights of all our type and more. Customize them and Bootstrap adapts.

====================
ICI COMMENCER
====================

#### Inline text elements

##### Marked text

For highlighting a run of text due to its relevance in another context, use the `<mark>` tag.

    Example
    You can use the mark tag to highlight text.

    ```html   
    You can use the mark tag to <mark>highlight</mark> text.
    ```

##### Deleted text

For indicating blocks of text that have been deleted use the <del> tag.

This line of text is meant to be treated as deleted text.


<del>This line of text is meant to be treated as deleted text.</del>

##### Strikethrough text

For indicating blocks of text that are no longer relevant use the <s> tag.

This line of text is meant to be treated as no longer accurate.


<s>This line of text is meant to be treated as no longer accurate.</s>

##### Inserted text

For indicating additions to the document use the <ins> tag.

This line of text is meant to be treated as an addition to the document.


<ins>This line of text is meant to be treated as an addition to the document.</ins>

##### Underlined text

To underline text use the <u> tag.

This line of text will render as underlined


<u>This line of text will render as underlined</u>

Make use of HTML's default emphasis tags with lightweight styles.

##### Small text

For de-emphasizing inline or blocks of text, use the <small> tag to set text at 85% the size of the parent. Heading elements receive their own font-size for nested <small> elements.

You may alternatively use an inline element with .small in place of any <small>.

This line of text is meant to be treated as fine print.


<small>This line of text is meant to be treated as fine print.</small>

##### Bold

For emphasizing a snippet of text with a heavier font-weight.

The following snippet of text is rendered as bold text.


<strong>rendered as bold text</strong>

##### Italics

For emphasizing a snippet of text with italics.

The following snippet of text is rendered as italicized text.


<em>rendered as italicized text</em>

> **Alternate elements**
>
>> Feel free to use <b> and <i> in HTML5. <b> is meant to highlight words or phrases without conveying additional importance while <i> is mostly for voice, technical terms, etc.

#### Alignment classes

Easily realign text to components with text alignment classes.

Left aligned text.

Center aligned text.

Right aligned text.

Justified text.

No wrap text.


<p class="text-left">Left aligned text.</p>
<p class="text-center">Center aligned text.</p>
<p class="text-right">Right aligned text.</p>
<p class="text-justify">Justified text.</p>
<p class="text-nowrap">No wrap text.</p>

#### Transformation classes

Transform text in components with text capitalization classes.

Lowercased text.

Uppercased text.

Capitalized text.


<p class="text-lowercase">Lowercased text.</p>
<p class="text-uppercase">Uppercased text.</p>
<p class="text-capitalize">Capitalized text.</p>

#### Abbreviations

Stylized implementation of HTML's <abbr> element for abbreviations and acronyms to show the expanded version on hover. Abbreviations with a title attribute have a light dotted bottom border and a help cursor on hover, providing additional context on hover and to users of assistive technologies.

##### Basic abbreviation

An abbreviation of the word attribute is attr.


<abbr title="attribute">attr</abbr>

###### Initialism

Add .initialism to an abbreviation for a slightly smaller font-size.

HTML is the best thing since sliced bread.


<abbr title="HyperText Markup Language" class="initialism">HTML</abbr>

#### Addresses

Present contact information for the nearest ancestor or the entire body of work. Preserve formatting by ending all lines with <br>.
Twitter, Inc.
1355 Market Street, Suite 900
San Francisco, CA 94103
P: (123) 456-7890
Full Name
first.last@example.com


<address>
  <strong>Twitter, Inc.</strong><br>
  1355 Market Street, Suite 900<br>
  San Francisco, CA 94103<br>
  <abbr title="Phone">P:</abbr> (123) 456-7890
</address>

<address>
  <strong>Full Name</strong><br>
  <a href="mailto:#">first.last@example.com</a>
</address>

#### Blockquotes

For quoting blocks of content from another source within your document.

##### Default blockquote

Wrap <blockquote> around any HTML as the quote. For straight quotes, we recommend a <p>.

    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.



<blockquote>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
</blockquote>

##### Blockquote options

Style and content changes for simple variations on a standard <blockquote>.

###### Naming a source

Add a <footer> for identifying the source. Wrap the name of the source work in <cite>.

    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.
    Someone famous in Source Title



<blockquote>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
  <footer>Someone famous in <cite title="Source Title">Source Title</cite></footer>
</blockquote>

###### Alternate displays

Add .blockquote-reverse for a blockquote with right-aligned content.

    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.
    Someone famous in Source Title



<blockquote class="blockquote-reverse">
  ...
</blockquote>

#### Lists

##### Unordered

A list of items in which the order does not explicitly matter.

    Lorem ipsum dolor sit amet
    Consectetur adipiscing elit
    Integer molestie lorem at massa
    Facilisis in pretium nisl aliquet
    Nulla volutpat aliquam velit
        Phasellus iaculis neque
        Purus sodales ultricies
        Vestibulum laoreet porttitor sem
        Ac tristique libero volutpat at
    Faucibus porta lacus fringilla vel
    Aenean sit amet erat nunc
    Eget porttitor lorem



<ul>
  <li>...</li>
</ul>

##### Ordered

A list of items in which the order does explicitly matter.

    Lorem ipsum dolor sit amet
    Consectetur adipiscing elit
    Integer molestie lorem at massa
    Facilisis in pretium nisl aliquet
    Nulla volutpat aliquam velit
    Faucibus porta lacus fringilla vel
    Aenean sit amet erat nunc
    Eget porttitor lorem



<ol>
  <li>...</li>
</ol>

##### Unstyled

Remove the default list-style and left margin on list items (immediate children only). This only applies to immediate children list items, meaning you will need to add the class for any nested lists as well.

    Lorem ipsum dolor sit amet
    Consectetur adipiscing elit
    Integer molestie lorem at massa
    Facilisis in pretium nisl aliquet
    Nulla volutpat aliquam velit
        Phasellus iaculis neque
        Purus sodales ultricies
        Vestibulum laoreet porttitor sem
        Ac tristique libero volutpat at
    Faucibus porta lacus fringilla vel
    Aenean sit amet erat nunc
    Eget porttitor lorem



<ul class="list-unstyled">
  <li>...</li>
</ul>

##### Inline

Place all list items on a single line with display: inline-block; and some light padding.

    Lorem ipsum Phasellus iaculis Nulla volutpat 



<ul class="list-inline">
  <li>...</li>
</ul>

##### Description

A list of terms with their associated descriptions.

Description lists
    A description list is perfect for defining terms.
Euismod
    Vestibulum id ligula porta felis euismod semper eget lacinia odio sem nec elit.
    Donec id elit non mi porta gravida at eget metus.
Malesuada porta
    Etiam porta sem malesuada magna mollis euismod.



<dl>
  <dt>...</dt>
  <dd>...</dd>
</dl>

###### Horizontal description

Make terms and descriptions in <dl> line up side-by-side. Starts off stacked like default <dl>s, but when the navbar expands, so do these.

Description lists
    A description list is perfect for defining terms.
Euismod
    Vestibulum id ligula porta felis euismod semper eget lacinia odio sem nec elit.
    Donec id elit non mi porta gravida at eget metus.
Malesuada porta
    Etiam porta sem malesuada magna mollis euismod.
Felis euismod semper eget lacinia
    Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus.



<dl class="dl-horizontal">
  <dt>...</dt>
  <dd>...</dd>
</dl>

> **Auto-truncating**
>
>>Horizontal description lists will truncate terms that are too long to fit in the left column with text-overflow. In narrower viewports, they will change to the default stacked layout.

### Code

#### Inline

Wrap inline snippets of code with <code>.
For example, <section> should be wrapped as inline.


For example, <code>&lt;section&gt;</code> should be wrapped as inline.

#### User input

Use the <kbd> to indicate input that is typically entered via keyboard.
To switch directories, type cd followed by the name of the directory.
To edit settings, press ctrl + ,


To switch directories, type <kbd>cd</kbd> followed by the name of the directory.<br>
To edit settings, press <kbd><kbd>ctrl</kbd> + <kbd>,</kbd></kbd>

#### Basic block

Use <pre> for multiple lines of code. Be sure to escape any angle brackets in the code for proper rendering.

<p>Sample text here...</p>



<pre>&lt;p&gt;Sample text here...&lt;/p&gt;</pre>

You may optionally add the .pre-scrollable class, which will set a max-height of 350px and provide a y-axis scrollbar.

#### Variables

For indicating variables use the <var> tag.

y = mx + b


<var>y</var> = <var>m</var><var>x</var> + <var>b</var>

#### Sample output

For indicating blocks sample output from a program use the <samp> tag.

This text is meant to be treated as sample output from a computer program.


<samp>This text is meant to be treated as sample output from a computer program.</samp>

### Tables

#### Basic example

For basic styling—light padding and only horizontal dividers—add the base class .table to any <table>. It may seem super redundant, but given the widespread use of tables for other plugins like calendars and date pickers, we've opted to isolate our custom table styles.
Optional table caption. # 	First Name 	Last Name 	Username
1 	Mark 	Otto 	@mdo
2 	Jacob 	Thornton 	@fat
3 	Larry 	the Bird 	@twitter


<table class="table">
  ...
</table>

####  Striped rows

Use .table-striped to add zebra-striping to any table row within the <tbody>.
Cross-browser compatibility

Striped tables are styled via the :nth-child CSS selector, which is not available in Internet Explorer 8.
# 	First Name 	Last Name 	Username
1 	Mark 	Otto 	@mdo
2 	Jacob 	Thornton 	@fat
3 	Larry 	the Bird 	@twitter


<table class="table table-striped">
  ...
</table>

#### Bordered table

Add .table-bordered for borders on all sides of the table and cells.
# 	First Name 	Last Name 	Username
1 	Mark 	Otto 	@mdo
2 	Jacob 	Thornton 	@fat
3 	Larry 	the Bird 	@twitter


<table class="table table-bordered">
  ...
</table>

#### Hover rows

Add .table-hover to enable a hover state on table rows within a <tbody>.
# 	First Name 	Last Name 	Username
1 	Mark 	Otto 	@mdo
2 	Jacob 	Thornton 	@fat
3 	Larry 	the Bird 	@twitter


<table class="table table-hover">
  ...
</table>

#### Condensed table

Add .table-condensed to make tables more compact by cutting cell padding in half.
# 	First Name 	Last Name 	Username
1 	Mark 	Otto 	@mdo
2 	Jacob 	Thornton 	@fat
3 	Larry the Bird 	@twitter


<table class="table table-condensed">
  ...
</table>

#### Contextual classes

Use contextual classes to color table rows or individual cells.
Class 	Description
.active 	Applies the hover color to a particular row or cell
.success 	Indicates a successful or positive action
.info 	Indicates a neutral informative change or action
.warning 	Indicates a warning that might need attention
.danger 	Indicates a dangerous or potentially negative action
# 	Column heading 	Column heading 	Column heading
1 	Column content 	Column content 	Column content
2 	Column content 	Column content 	Column content
3 	Column content 	Column content 	Column content
4 	Column content 	Column content 	Column content
5 	Column content 	Column content 	Column content
6 	Column content 	Column content 	Column content
7 	Column content 	Column content 	Column content
8 	Column content 	Column content 	Column content
9 	Column content 	Column content 	Column content


<!-- On rows -->
<tr class="active">...</tr>
<tr class="success">...</tr>
<tr class="warning">...</tr>
<tr class="danger">...</tr>
<tr class="info">...</tr>

<!-- On cells (`td` or `th`) -->
<tr>
  <td class="active">...</td>
  <td class="success">...</td>
  <td class="warning">...</td>
  <td class="danger">...</td>
  <td class="info">...</td>
</tr>

> **Conveying meaning to assistive technologies**
>
>> Using color to add meaning to a table row or individual cell only provides a visual indication, which will not be conveyed to users of assistive technologies – such as screen readers. Ensure that information denoted by the color is either obvious from the content itself (the visible text in the relevant table row/cell), or is included through alternative means, such as additional text hidden with the .sr-only class.

#### Responsive tables

Create responsive tables by wrapping any .table in .table-responsive to make them scroll horizontally on small devices (under 768px). When viewing on anything larger than 768px wide, you will not see any difference in these tables.

> **Vertical clipping/truncation**
>
>> Responsive tables make use of overflow-y: hidden, which clips off any content that goes beyond the bottom or top edges of the table. In particular, this can clip off dropdown menus and other third-party widgets.

> Firefox and fieldsets
>
>> Firefox has some awkward fieldset styling involving width that interferes with the responsive table. This cannot be overridden without a Firefox-specific hack that we don't provide in Bootstrap:


@-moz-document url-prefix() {
  fieldset { display: table-cell; }
}

For more information, read this Stack Overflow answer.
# 	Table heading 	Table heading 	Table heading 	Table heading 	Table heading 	Table heading
1 	Table cell 	Table cell 	Table cell 	Table cell 	Table cell 	Table cell
2 	Table cell 	Table cell 	Table cell 	Table cell 	Table cell 	Table cell
3 	Table cell 	Table cell 	Table cell 	Table cell 	Table cell 	Table cell
# 	Table heading 	Table heading 	Table heading 	Table heading 	Table heading 	Table heading
1 	Table cell 	Table cell 	Table cell 	Table cell 	Table cell 	Table cell
2 	Table cell 	Table cell 	Table cell 	Table cell 	Table cell 	Table cell
3 	Table cell 	Table cell 	Table cell 	Table cell 	Table cell 	Table cell


<div class="table-responsive">
  <table class="table">
    ...
  </table>
</div>

### Forms

#### Basic example

Individual form controls automatically receive some global styling. All textual <input>, <textarea>, and <select> elements with .form-control are set to width: 100%; by default. Wrap labels and controls in .form-group for optimum spacing.
Email address
Password
File input

Example block-level help text here.
Check me out


<form>
  <div class="form-group">
    <label for="exampleInputEmail1">Email address</label>
    <input type="email" class="form-control" id="exampleInputEmail1" placeholder="Email">
  </div>
  <div class="form-group">
    <label for="exampleInputPassword1">Password</label>
    <input type="password" class="form-control" id="exampleInputPassword1" placeholder="Password">
  </div>
  <div class="form-group">
    <label for="exampleInputFile">File input</label>
    <input type="file" id="exampleInputFile">
    <p class="help-block">Example block-level help text here.</p>
  </div>
  <div class="checkbox">
    <label>
      <input type="checkbox"> Check me out
    </label>
  </div>
  <button type="submit" class="btn btn-default">Submit</button>
</form>

> Don't mix form groups with input groups
>
>> Do not mix form groups directly with input groups. Instead, nest the input group inside of the form group.

#### Inline form

Add .form-inline to your form (which doesn't have to be a <form>) for left-aligned and inline-block controls. This only applies to forms within viewports that are at least 768px wide.

> May require custom widths
>
>> Inputs and selects have width: 100%; applied by default in Bootstrap. Within inline forms, we reset that to width: auto; so multiple controls can reside on the same line. Depending on your layout, additional custom widths may be required.

>Always add labels
>
>> Screen readers will have trouble with your forms if you don't include a label for every input. For these inline forms, you can hide the labels using the .sr-only class. There are further alternative methods of providing a label for assistive technologies, such as the aria-label, aria-labelledby or title attribute. If none of these is present, screen readers may resort to using the placeholder attribute, if present, but note that use of placeholder as a replacement for other labelling methods is not advised.

Name
Email


<form class="form-inline">
  <div class="form-group">
    <label for="exampleInputName2">Name</label>
    <input type="text" class="form-control" id="exampleInputName2" placeholder="Jane Doe">
  </div>
  <div class="form-group">
    <label for="exampleInputEmail2">Email</label>
    <input type="email" class="form-control" id="exampleInputEmail2" placeholder="jane.doe@example.com">
  </div>
  <button type="submit" class="btn btn-default">Send invitation</button>
</form>

Email address
Password
Remember me


<form class="form-inline">
  <div class="form-group">
    <label class="sr-only" for="exampleInputEmail3">Email address</label>
    <input type="email" class="form-control" id="exampleInputEmail3" placeholder="Email">
  </div>
  <div class="form-group">
    <label class="sr-only" for="exampleInputPassword3">Password</label>
    <input type="password" class="form-control" id="exampleInputPassword3" placeholder="Password">
  </div>
  <div class="checkbox">
    <label>
      <input type="checkbox"> Remember me
    </label>
  </div>
  <button type="submit" class="btn btn-default">Sign in</button>
</form>

Amount (in dollars)
$
.00


<form class="form-inline">
  <div class="form-group">
    <label class="sr-only" for="exampleInputAmount">Amount (in dollars)</label>
    <div class="input-group">
      <div class="input-group-addon">$</div>
      <input type="text" class="form-control" id="exampleInputAmount" placeholder="Amount">
      <div class="input-group-addon">.00</div>
    </div>
  </div>
  <button type="submit" class="btn btn-primary">Transfer cash</button>
</form>

#### Horizontal form

Use Bootstrap's predefined grid classes to align labels and groups of form controls in a horizontal layout by adding .form-horizontal to the form (which doesn't have to be a <form>). Doing so changes .form-groups to behave as grid rows, so no need for .row.
Email
Password
Remember me


<form class="form-horizontal">
  <div class="form-group">
    <label for="inputEmail3" class="col-sm-2 control-label">Email</label>
    <div class="col-sm-10">
      <input type="email" class="form-control" id="inputEmail3" placeholder="Email">
    </div>
  </div>
  <div class="form-group">
    <label for="inputPassword3" class="col-sm-2 control-label">Password</label>
    <div class="col-sm-10">
      <input type="password" class="form-control" id="inputPassword3" placeholder="Password">
    </div>
  </div>
  <div class="form-group">
    <div class="col-sm-offset-2 col-sm-10">
      <div class="checkbox">
        <label>
          <input type="checkbox"> Remember me
        </label>
      </div>
    </div>
  </div>
  <div class="form-group">
    <div class="col-sm-offset-2 col-sm-10">
      <button type="submit" class="btn btn-default">Sign in</button>
    </div>
  </div>
</form>

#### Supported controls

Examples of standard form controls supported in an example form layout.

##### Inputs

Most common form control, text-based input fields. Includes support for all HTML5 types: text, password, datetime, datetime-local, date, month, time, week, number, email, url, search, tel, and color.

> Type declaration required
>
>> Inputs will only be fully styled if their type is properly declared.


<input type="text" class="form-control" placeholder="Text input">

> Input groups
>
>> To add integrated text or buttons before and/or after any text-based <input>, check out the input group component.

##### Textarea

Form control which supports multiple lines of text. Change rows attribute as necessary.


<textarea class="form-control" rows="3"></textarea>

##### Checkboxes and radios

Checkboxes are for selecting one or several options in a list, while radios are for selecting one option from many.

Disabled checkboxes and radios are supported, but to provide a "not-allowed" cursor on hover of the parent <label>, you'll need to add the .disabled class to the parent .radio, .radio-inline, .checkbox, or .checkbox-inline.

###### Default (stacked)

Option one is this and that—be sure to include why it's great
Option two is disabled

Option one is this and that—be sure to include why it's great
Option two can be something else and selecting it will deselect option one
Option three is disabled


<div class="checkbox">
  <label>
    <input type="checkbox" value="">
    Option one is this and that&mdash;be sure to include why it's great
  </label>
</div>
<div class="checkbox disabled">
  <label>
    <input type="checkbox" value="" disabled>
    Option two is disabled
  </label>
</div>

<div class="radio">
  <label>
    <input type="radio" name="optionsRadios" id="optionsRadios1" value="option1" checked>
    Option one is this and that&mdash;be sure to include why it's great
  </label>
</div>
<div class="radio">
  <label>
    <input type="radio" name="optionsRadios" id="optionsRadios2" value="option2">
    Option two can be something else and selecting it will deselect option one
  </label>
</div>
<div class="radio disabled">
  <label>
    <input type="radio" name="optionsRadios" id="optionsRadios3" value="option3" disabled>
    Option three is disabled
  </label>
</div>

###### Inline checkboxes and radios

Use the .checkbox-inline or .radio-inline classes on a series of checkboxes or radios for controls that appear on the same line.
1 2 3

1 2 3


<label class="checkbox-inline">
  <input type="checkbox" id="inlineCheckbox1" value="option1"> 1
</label>
<label class="checkbox-inline">
  <input type="checkbox" id="inlineCheckbox2" value="option2"> 2
</label>
<label class="checkbox-inline">
  <input type="checkbox" id="inlineCheckbox3" value="option3"> 3
</label>

<label class="radio-inline">
  <input type="radio" name="inlineRadioOptions" id="inlineRadio1" value="option1"> 1
</label>
<label class="radio-inline">
  <input type="radio" name="inlineRadioOptions" id="inlineRadio2" value="option2"> 2
</label>
<label class="radio-inline">
  <input type="radio" name="inlineRadioOptions" id="inlineRadio3" value="option3"> 3
</label>

##### Checkboxes and radios without label text

Should you have no text within the <label>, the input is positioned as you'd expect. Currently only works on non-inline checkboxes and radios. Remember to still provide some form of label for assistive technologies (for instance, using aria-label).


<div class="checkbox">
  <label>
    <input type="checkbox" id="blankCheckbox" value="option1" aria-label="...">
  </label>
</div>
<div class="radio">
  <label>
    <input type="radio" name="blankRadio" id="blankRadio1" value="option1" aria-label="...">
  </label>
</div>

##### Selects

Note that many native select menus—namely in Safari and Chrome—have rounded corners that cannot be modified via border-radius properties.


<select class="form-control">
  <option>1</option>
  <option>2</option>
  <option>3</option>
  <option>4</option>
  <option>5</option>
</select>

For <select> controls with the multiple attribute, multiple options are shown by default.


<select multiple class="form-control">
  <option>1</option>
  <option>2</option>
  <option>3</option>
  <option>4</option>
  <option>5</option>
</select>

#### Static control

When you need to place plain text next to a form label within a form, use the .form-control-static class on a <p>.
Email

email@example.com
Password


<form class="form-horizontal">
  <div class="form-group">
    <label class="col-sm-2 control-label">Email</label>
    <div class="col-sm-10">
      <p class="form-control-static">email@example.com</p>
    </div>
  </div>
  <div class="form-group">
    <label for="inputPassword" class="col-sm-2 control-label">Password</label>
    <div class="col-sm-10">
      <input type="password" class="form-control" id="inputPassword" placeholder="Password">
    </div>
  </div>
</form>

Email

email@example.com
Password


<form class="form-inline">
  <div class="form-group">
    <label class="sr-only">Email</label>
    <p class="form-control-static">email@example.com</p>
  </div>
  <div class="form-group">
    <label for="inputPassword2" class="sr-only">Password</label>
    <input type="password" class="form-control" id="inputPassword2" placeholder="Password">
  </div>
  <button type="submit" class="btn btn-default">Confirm identity</button>
</form>

#### Focus state

We remove the default outline styles on some form controls and apply a box-shadow in its place for :focus.
Demo :focus state

The above example input uses custom styles in our documentation to demonstrate the :focus state on a .form-control.

#### Disabled state

Add the disabled boolean attribute on an input to prevent user interactions. Disabled inputs appear lighter and add a not-allowed cursor.


<input class="form-control" id="disabledInput" type="text" placeholder="Disabled input here..." disabled>

##### Disabled fieldsets

Add the disabled attribute to a <fieldset> to disable all the controls within the <fieldset> at once.

> Caveat about link functionality of <a>
>
>> By default, browsers will treat all native form controls (<input>, <select> and <button> elements) inside a <fieldset disabled> as disabled, preventing both keyboard and mouse interactions on them. However, if your form also includes <a ... class="btn btn-*"> elements, these will only be given a style of pointer-events: none. As noted in the section about disabled state for buttons (and specifically in the sub-section for anchor elements), this CSS property is not yet standardized and isn't fully supported in Opera 18 and below, or in Internet Explorer 11, and won't prevent keyboard users from being able to focus or activate these links. So to be safe, use custom JavaScript to disable such links.

> Cross-browser compatibility
>
>> While Bootstrap will apply these styles in all browsers, Internet Explorer 11 and below don't fully support the disabled attribute on a <fieldset>. Use custom JavaScript to disable the fieldset in these browsers.
Disabled input
Disabled select menu
Can't check this


<form>
  <fieldset disabled>
    <div class="form-group">
      <label for="disabledTextInput">Disabled input</label>
      <input type="text" id="disabledTextInput" class="form-control" placeholder="Disabled input">
    </div>
    <div class="form-group">
      <label for="disabledSelect">Disabled select menu</label>
      <select id="disabledSelect" class="form-control">
        <option>Disabled select</option>
      </select>
    </div>
    <div class="checkbox">
      <label>
        <input type="checkbox"> Can't check this
      </label>
    </div>
    <button type="submit" class="btn btn-primary">Submit</button>
  </fieldset>
</form>

#### Readonly state

Add the readonly boolean attribute on an input to prevent modification of the input's value. Read-only inputs appear lighter (just like disabled inputs), but retain the standard cursor.


<input class="form-control" type="text" placeholder="Readonly input here…" readonly>

#### Help text

Block level help text for form controls.
Associating help text with form controls

Help text should be explicitly associated with the form control it relates to using the aria-describedby attribute. This will ensure that assistive technologies – such as screen readers – will announce this help text when the user focuses or enters the control.
Input with help text
A block of help text that breaks onto a new line and may extend beyond one line.


<label class="sr-only" for="inputHelpBlock">Input with help text</label>
<input type="text" id="inputHelpBlock" class="form-control" aria-describedby="helpBlock">
...
<span id="helpBlock" class="help-block">A block of help text that breaks onto a new line and may extend beyond one line.</span>

#### Validation states

Bootstrap includes validation styles for error, warning, and success states on form controls. To use, add .has-warning, .has-error, or .has-success to the parent element. Any .control-label, .form-control, and .help-block within that element will receive the validation styles.

> **Conveying validation state to assistive technologies and colorblind users**
>
>> Using these validation styles to denote the state of a form control only provides a visual, color-based indication, which will not be conveyed to users of assistive technologies - such as screen readers - or to colorblind users.
>> Ensure that an alternative indication of state is also provided. For instance, you can include a hint about state in the form control's <label> text itself (as is the case in the following code example), include a Glyphicon (with appropriate alternative text using the .sr-only class - see the Glyphicon examples), or by providing an additional help text block. Specifically for assistive technologies, invalid form controls can also be assigned an aria-invalid="true" attribute.

![IMG](IMG)

```
<div class="form-group has-success">
  <label class="control-label" for="inputSuccess1">Input with success</label>
  <input type="text" class="form-control" id="inputSuccess1" aria-describedby="helpBlock2">
  <span id="helpBlock2" class="help-block">A block of help text that breaks onto a new line and may extend beyond one line.</span>
</div>
<div class="form-group has-warning">
  <label class="control-label" for="inputWarning1">Input with warning</label>
  <input type="text" class="form-control" id="inputWarning1">
</div>
<div class="form-group has-error">
  <label class="control-label" for="inputError1">Input with error</label>
  <input type="text" class="form-control" id="inputError1">
</div>
<div class="has-success">
  <div class="checkbox">
    <label>
      <input type="checkbox" id="checkboxSuccess" value="option1">
      Checkbox with success
    </label>
  </div>
</div>
<div class="has-warning">
  <div class="checkbox">
    <label>
      <input type="checkbox" id="checkboxWarning" value="option1">
      Checkbox with warning
    </label>
  </div>
</div>
<div class="has-error">
  <div class="checkbox">
    <label>
      <input type="checkbox" id="checkboxError" value="option1">
      Checkbox with error
    </label>
  </div>
</div>
```

##### With optional icons

You can also add optional feedback icons with the addition of `.has-feedback` and the right icon.

**Feedback icons only work with textual `<input class="form-control">` elements.**

> **Icons, labels, and input groups**
>
>> Manual positioning of feedback icons is required for inputs without a label and for input groups with an add-on on the right. You are strongly encouraged to provide labels for all inputs for accessibility reasons. If you wish to prevent labels from being displayed, hide them with the `.sr-only` class. If you must do without labels, adjust the `top` value of the feedback icon. For input groups, adjust the `right` value to an appropriate pixel value depending on the width of your addon.

> **Conveying the icon's meaning to assistive technologies**
>
>> To ensure that assistive technologies – such as screen readers – correctly convey the meaning of an icon, additional hidden text should be included with the `.sr-only` class and explicitly associated with the form control it relates to using `aria-describedby`. Alternatively, ensure that the meaning (for instance, the fact that there is a warning for a particular text entry field) is conveyed in some other form, such as changing the text of the actual `<label>` associated with the form control.
>> Although the following examples already mention the validation state of their respective form controls in the `<label>` text itself, the above technique (using `.sr-only` text and `aria-describedby`) has been included for illustrative purposes.

![IMG](IMG)

```
<div class="form-group has-success has-feedback">
  <label class="control-label" for="inputSuccess2">Input with success</label>
  <input type="text" class="form-control" id="inputSuccess2" aria-describedby="inputSuccess2Status">
  <span class="glyphicon glyphicon-ok form-control-feedback" aria-hidden="true"></span>
  <span id="inputSuccess2Status" class="sr-only">(success)</span>
</div>
<div class="form-group has-warning has-feedback">
  <label class="control-label" for="inputWarning2">Input with warning</label>
  <input type="text" class="form-control" id="inputWarning2" aria-describedby="inputWarning2Status">
  <span class="glyphicon glyphicon-warning-sign form-control-feedback" aria-hidden="true"></span>
  <span id="inputWarning2Status" class="sr-only">(warning)</span>
</div>
<div class="form-group has-error has-feedback">
  <label class="control-label" for="inputError2">Input with error</label>
  <input type="text" class="form-control" id="inputError2" aria-describedby="inputError2Status">
  <span class="glyphicon glyphicon-remove form-control-feedback" aria-hidden="true"></span>
  <span id="inputError2Status" class="sr-only">(error)</span>
</div>
<div class="form-group has-success has-feedback">
  <label class="control-label" for="inputGroupSuccess1">Input group with success</label>
  <div class="input-group">
    <span class="input-group-addon">@</span>
    <input type="text" class="form-control" id="inputGroupSuccess1" aria-describedby="inputGroupSuccess1Status">
  </div>
  <span class="glyphicon glyphicon-ok form-control-feedback" aria-hidden="true"></span>
  <span id="inputGroupSuccess1Status" class="sr-only">(success)</span>
</div>
```

###### Optional icons in horizontal and inline forms

![IMG](IMG)

```
<form class="form-horizontal">
  <div class="form-group has-success has-feedback">
    <label class="control-label col-sm-3" for="inputSuccess3">Input with success</label>
    <div class="col-sm-9">
      <input type="text" class="form-control" id="inputSuccess3" aria-describedby="inputSuccess3Status">
      <span class="glyphicon glyphicon-ok form-control-feedback" aria-hidden="true"></span>
      <span id="inputSuccess3Status" class="sr-only">(success)</span>
    </div>
  </div>
  <div class="form-group has-success has-feedback">
    <label class="control-label col-sm-3" for="inputGroupSuccess2">Input group with success</label>
    <div class="col-sm-9">
      <div class="input-group">
        <span class="input-group-addon">@</span>
        <input type="text" class="form-control" id="inputGroupSuccess2" aria-describedby="inputGroupSuccess2Status">
      </div>
      <span class="glyphicon glyphicon-ok form-control-feedback" aria-hidden="true"></span>
      <span id="inputGroupSuccess2Status" class="sr-only">(success)</span>
    </div>
  </div>
</form>
```

![IMG](IMG)

```
<form class="form-inline">
  <div class="form-group has-success has-feedback">
    <label class="control-label" for="inputSuccess4">Input with success</label>
    <input type="text" class="form-control" id="inputSuccess4" aria-describedby="inputSuccess4Status">
    <span class="glyphicon glyphicon-ok form-control-feedback" aria-hidden="true"></span>
    <span id="inputSuccess4Status" class="sr-only">(success)</span>
  </div>
</form>
<form class="form-inline">
  <div class="form-group has-success has-feedback">
    <label class="control-label" for="inputGroupSuccess3">Input group with success</label>
    <div class="input-group">
      <span class="input-group-addon">@</span>
      <input type="text" class="form-control" id="inputGroupSuccess3" aria-describedby="inputGroupSuccess3Status">
    </div>
    <span class="glyphicon glyphicon-ok form-control-feedback" aria-hidden="true"></span>
    <span id="inputGroupSuccess3Status" class="sr-only">(success)</span>
  </div>
</form>
```

###### Optional icons with hidden `.sr-only` labels

If you use the .sr-only class to hide a form control's <label> (rather than using other labelling options, such as the aria-label attribute), Bootstrap will automatically adjust the position of the icon once it's been added.

![IMG](IMG)

```
<div class="form-group has-success has-feedback">
  <label class="control-label sr-only" for="inputSuccess5">Hidden label</label>
  <input type="text" class="form-control" id="inputSuccess5" aria-describedby="inputSuccess5Status">
  <span class="glyphicon glyphicon-ok form-control-feedback" aria-hidden="true"></span>
  <span id="inputSuccess5Status" class="sr-only">(success)</span>
</div>
<div class="form-group has-success has-feedback">
  <label class="control-label sr-only" for="inputGroupSuccess4">Input group with success</label>
  <div class="input-group">
    <span class="input-group-addon">@</span>
    <input type="text" class="form-control" id="inputGroupSuccess4" aria-describedby="inputGroupSuccess4Status">
  </div>
  <span class="glyphicon glyphicon-ok form-control-feedback" aria-hidden="true"></span>
  <span id="inputGroupSuccess4Status" class="sr-only">(success)</span>
</div>
```

#### Control sizing

Set heights using classes like `.input-lg`, and set widths using grid column classes like `.col-lg-*`.

##### Height sizing

Create taller or shorter form controls that match button sizes.

![IMG](IMG)

```
<input class="form-control input-lg" type="text" placeholder=".input-lg">
<input class="form-control" type="text" placeholder="Default input">
<input class="form-control input-sm" type="text" placeholder=".input-sm">

<select class="form-control input-lg">...</select>
<select class="form-control">...</select>
<select class="form-control input-sm">...</select>
```

##### Horizontal form group sizes

Quickly size labels and form controls within `.form-horizontal` by adding `.form-group-lg` or `.form-group-sm`.

![IMG](IMG)

```
<form class="form-horizontal">
  <div class="form-group form-group-lg">
    <label class="col-sm-2 control-label" for="formGroupInputLarge">Large label</label>
    <div class="col-sm-10">
      <input class="form-control" type="text" id="formGroupInputLarge" placeholder="Large input">
    </div>
  </div>
  <div class="form-group form-group-sm">
    <label class="col-sm-2 control-label" for="formGroupInputSmall">Small label</label>
    <div class="col-sm-10">
      <input class="form-control" type="text" id="formGroupInputSmall" placeholder="Small input">
    </div>
  </div>
</form>
```

##### Column sizing

Wrap inputs in grid columns, or any custom parent element, to easily enforce desired widths.

![IMG](IMG)

```
<div class="row">
  <div class="col-xs-2">
    <input type="text" class="form-control" placeholder=".col-xs-2">
  </div>
  <div class="col-xs-3">
    <input type="text" class="form-control" placeholder=".col-xs-3">
  </div>
  <div class="col-xs-4">
    <input type="text" class="form-control" placeholder=".col-xs-4">
  </div>
</div>
```

### Buttons

#### Button tags

Use the button classes on an `<a>`, `<button>`, or `<input>` element.

![IMG](IMG)

```
<a class="btn btn-default" href="#" role="button">Link</a>
<button class="btn btn-default" type="submit">Button</button>
<input class="btn btn-default" type="button" value="Input">
<input class="btn btn-default" type="submit" value="Submit">
```

> **Context-specific usage**
>
>> While button classes can be used on `<a>` and `<button>` elements, only `<button>` elements are supported within our nav and navbar components.

> **Links acting as buttons**
> 
>> If the `<a>` elements are used to act as buttons – triggering in-page functionality, rather than navigating to another document or section within the current page – they should also be given an appropriate `role="button"`.

> **Cross-browser rendering**
>
>> As a best practice, **we highly recommend using the `<button>` element whenever possible** to ensure matching cross-browser rendering.
>> Among other things, there's a bug in Firefox <30 that prevents us from setting the `line-height` of `<input>`-based buttons, causing them to not exactly match the height of other buttons on Firefox.

#### Options

Use any of the available button classes to quickly create a styled button.

![IMG](IMG)

```
<!-- Standard button -->
<button type="button" class="btn btn-default">Default</button>
<!-- Provides extra visual weight and identifies the primary action in a set of buttons -->
<button type="button" class="btn btn-primary">Primary</button>
<!-- Indicates a successful or positive action -->
<button type="button" class="btn btn-success">Success</button>
<!-- Contextual button for informational alert messages -->
<button type="button" class="btn btn-info">Info</button>
<!-- Indicates caution should be taken with this action -->
<button type="button" class="btn btn-warning">Warning</button>
<!-- Indicates a dangerous or potentially negative action -->
<button type="button" class="btn btn-danger">Danger</button>
<!-- Deemphasize a button by making it look like a link while maintaining button behavior -->
<button type="button" class="btn btn-link">Link</button>
```

> **Conveying meaning to assistive technologies**
>
>> Using color to add meaning to a button only provides a visual indication, which will not be conveyed to users of assistive technologies – such as screen readers. Ensure that information denoted by the color is either obvious from the content itself (the visible text of the button), or is included through alternative means, such as additional text hidden with the `.sr-only` class.

#### Sizes

Fancy larger or smaller buttons? Add `.btn-lg`, `.btn-sm`, or `.btn-xs` for additional sizes.

![IMG](IMG)

```
<p>
  <button type="button" class="btn btn-primary btn-lg">Large button</button>
  <button type="button" class="btn btn-default btn-lg">Large button</button>
</p>
<p>
  <button type="button" class="btn btn-primary">Default button</button>
  <button type="button" class="btn btn-default">Default button</button>
</p>
<p>
  <button type="button" class="btn btn-primary btn-sm">Small button</button>
  <button type="button" class="btn btn-default btn-sm">Small button</button>
</p>
<p>
  <button type="button" class="btn btn-primary btn-xs">Extra small button</button>
  <button type="button" class="btn btn-default btn-xs">Extra small button</button>
</p>
```

Create block level buttons—those that span the full width of a parent— by adding `.btn-block`.

![IMG](IMG)

```
<button type="button" class="btn btn-primary btn-lg btn-block">Block level button</button>
<button type="button" class="btn btn-default btn-lg btn-block">Block level button</button>
```

#### Active state

Buttons will appear pressed (with a darker background, darker border, and inset shadow) when active. For `<button>` elements, this is done via `:active`. For `<a>` elements, it's done with `.active`. However, you may use `.active` on `<button>`s (and include the `aria-pressed="true"` attribute) should you need to replicate the active state programmatically.

##### Button element

No need to add `:active` as it's a pseudo-class, but if you need to force the same appearance, go ahead and add `.active`.

![IMG](IMG)

```
<button type="button" class="btn btn-primary btn-lg active">Primary button</button>
<button type="button" class="btn btn-default btn-lg active">Button</button>
```

##### Anchor element

Add the `.active` class to `<a>` buttons.

![IMG](IMG)

```
<a href="#" class="btn btn-primary btn-lg active" role="button">Primary link</a>
<a href="#" class="btn btn-default btn-lg active" role="button">Link</a>
```

#### Disabled state

Make buttons look unclickable by fading them back with `opacity`.

##### Button element

Add the `disabled` attribute to `<button>` buttons.

![IMG](IMG)

```
<button type="button" class="btn btn-lg btn-primary" disabled="disabled">Primary button</button>
<button type="button" class="btn btn-default btn-lg" disabled="disabled">Button</button>
```

> **Cross-browser compatibility**
>
>> If you add the `disabled` attribute to a `<button>`, Internet Explorer 9 and below will render text gray with a nasty text-shadow that we cannot fix.

#### Anchor element

Add the .disabled class to `<a>` buttons.

![IMG](IMG)

```
<a href="#" class="btn btn-primary btn-lg disabled" role="button">Primary link</a>
<a href="#" class="btn btn-default btn-lg disabled" role="button">Link</a>
```

We use .disabled as a utility class here, similar to the common `.active` class, so no prefix is required.

> **Link functionality caveat**
>
>> This class uses `pointer-events: none` to try to disable the link functionality of `<a>`s, but that CSS property is not yet standardized and isn't fully supported in Opera 18 and below, or in Internet Explorer 11. In addition, even in browsers that do support `pointer-events: none`, keyboard navigation remains unaffected, meaning that sighted keyboard users and users of assistive technologies will still be able to activate these links. So to be safe, use custom JavaScript to disable such links.

### Images

#### Responsive images

Images in Bootstrap 3 can be made responsive-friendly via the addition of the `.img-responsive` class. This applies `max-width: 100%;`, `height: auto;` and `display: block;` to the image so that it scales nicely to the parent element.

To center images which use the `.img-responsive` class, use `.center-block` instead of `.text-center`. [See the helper classes section](https://getbootstrap.com/docs/3.3/css/#helper-classes-center) for more details about `.center-block` usage.

> **SVG images and IE 8-10**
>
>> In Internet Explorer 8-10, SVG images with `.img-responsive` are disproportionately sized. To fix this, add `width: 100% \9;` where necessary. Bootstrap doesn't apply this automatically as it causes complications to other image formats.

```
<img src="..." class="img-responsive" alt="Responsive image">
```

#### Image shapes

Add classes to an `<img>` element to easily style images in any project.

> **Cross-browser compatibility**
>
>> Keep in mind that Internet Explorer 8 lacks support for rounded corners.

![IMG](IMG)

```
<img src="..." alt="..." class="img-rounded">
<img src="..." alt="..." class="img-circle">
<img src="..." alt="..." class="img-thumbnail">
```

### Helper classes

#### Contextual colors

Convey meaning through color with a handful of emphasis utility classes. These may also be applied to links and will darken on hover just like our default link styles.

![IMG](IMG)

```
<p class="text-muted">...</p>
<p class="text-primary">...</p>
<p class="text-success">...</p>
<p class="text-info">...</p>
<p class="text-warning">...</p>
<p class="text-danger">...</p>
```

> **Dealing with specificity**
>
>> Sometimes emphasis classes cannot be applied due to the specificity of another selector. In most cases, a sufficient workaround is to wrap your text in a <span> with the class.

> **Conveying meaning to assistive technologies**
>
> Using color to add meaning only provides a visual indication, which will not be conveyed to users of assistive technologies – such as screen readers. Ensure that information denoted by the color is either obvious from the content itself (the contextual colors are only used to reinforce meaning that is already present in the text/markup), or is included through alternative means, such as additional text hidden with the .sr-only class.

#### Contextual backgrounds

Similar to the contextual text color classes, easily set the background of an element to any contextual class. Anchor components will darken on hover, just like the text classes.

![IMG](IMG)

```
<p class="bg-primary">...</p>
<p class="bg-success">...</p>
<p class="bg-info">...</p>
<p class="bg-warning">...</p>
<p class="bg-danger">...</p>
```

> **Dealing with specificity**
>
>> Sometimes contextual background classes cannot be applied due to the specificity of another selector. In some cases, a sufficient workaround is to wrap your element's content in a <div> with the class.

> **Conveying meaning to assistive technologies**
>
>> As with contextual colors, ensure that any meaning conveyed through color is also conveyed in a format that is not purely presentational.

#### Close icon

Use the generic close icon for dismissing content like modals and alerts.


```
<button type="button" class="close" aria-label="Close"><span aria-hidden="true">&times;</span></button>
```

#### Carets

Use carets to indicate dropdown functionality and direction. Note that the default caret will reverse automatically in [dropup menus](https://getbootstrap.com/docs/3.3/components/#btn-dropdowns-dropup).

![IMG](IMG)

```
<span class="caret"></span>
```

#### Quick floats

Float an element to the left or right with a class. `!important` is included to avoid specificity issues. Classes can also be used as mixins.

```
<div class="pull-left">...</div>
<div class="pull-right">...</div>
```

```
// Classes
.pull-left {
  float: left !important;
}
.pull-right {
  float: right !important;
}
// Usage as mixins
.element {
  .pull-left();
}
.another-element {
  .pull-right();
}
```

> **Not for use in navbars**
>
>> To align components in navbars with utility classes, use `.navbar-left` or `.navbar-right` instead. [See the navbar docs for details](https://getbootstrap.com/docs/3.3/components/#navbar-component-alignment).

#### Center content blocks

Set an element to `display: block` and center via `margin`. Available as a mixin and class.

```
<div class="center-block">...</div>
```

```
// Class
.center-block {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
// Usage as a mixin
.element {
  .center-block();
}
```

#### Clearfix

Easily clear `floats` by adding `.clearfix` **to the parent element**. Utilizes [the micro clearfix](http://nicolasgallagher.com/micro-clearfix-hack/) as popularized by Nicolas Gallagher. Can also be used as a mixin.

```
<!-- Usage as a class -->
<div class="clearfix">...</div>
```

```
// Mixin itself
.clearfix() {
  &:before,
  &:after {
    content: " ";
    display: table;
  }
  &:after {
    clear: both;
  }
}

// Usage as a mixin
.element {
  .clearfix();
}
```

#### Showing and hiding content

Force an element to be shown or hidden (**including for screen readers**) with the use of `.show` and `.hidden` classes. These classes use `!important` to avoid specificity conflicts, just like the quick floats. They are only available for block level toggling. They can also be used as mixins.

`.hide` is available, but it does not always affect screen readers and is **deprecated** as of v3.0.1. Use .hidden or `.sr-only` instead.

Furthermore, `.invisible` can be used to toggle only the visibility of an element, meaning its `display` is not modified and the element can still affect the flow of the document.

```
<div class="show">...</div>
<div class="hidden">...</div>
```

```
// Classes
.show {
  display: block !important;
}
.hidden {
  display: none !important;
}
.invisible {
  visibility: hidden;
}

// Usage as mixins
.element {
  .show();
}
.another-element {
  .hidden();
}
```

#### Screen reader and keyboard navigation content

Hide an element to all devices **except screen readers** with `.sr-only.` Combine `.sr-only` with `.sr-only-focusable` to show the element again when it's focused (e.g. by a keyboard-only user). Necessary for following [accessibility best practices](https://getbootstrap.com/docs/3.3/getting-started/#accessibility). Can also be used as mixins.

```
<a class="sr-only sr-only-focusable" href="#content">Skip to main content</a>
```

```
// Usage as a mixin
.skip-navigation {
  .sr-only();
  .sr-only-focusable();
}
```

#### Image replacement

Utilize the `.text-hide` class or mixin to help replace an element's text content with a background image.

```
<h1 class="text-hide">Custom heading</h1>
```

```
// Usage as a mixin
.heading {
  .text-hide();
}
```

### Responsive utilities

**For faster mobile-friendly development, use these utility classes for showing and hiding content by device via media query. Also included are utility classes for toggling content when printed.**

Try to use these on a limited basis and avoid creating entirely different versions of the same site. Instead, use them to complement each device's presentation.

#### Available classes

Use a single or combination of the available classes for toggling content across viewport breakpoints.

| | Extra small devices Phones (<768px) | Small devices Tablets (≥768px) | Medium devices Desktops (≥992px) | Large devices Desktops (≥1200px) |
|----|----|----|----|----|
| `.visible-xs-*` | Visible | Hidden | Hidden | Hidden |
| `.visible-sm-*` | Hidden | Visible | Hidden | Hidden |
| `.visible-md-*` | Hidden | Hidden | Visible | Hidden |
| `.visible-lg-*` | Hidden | Hidden | Hidden | Visible |
| `.hidden-xs` | Hidden | Visible | Visible | Visible |
| `.hidden-sm` | Visible | Hidden | Visible | Visible |
| `.hidden-md` | Visible | Visible | Hidden | Visible |
| `.hidden-lg` | Visible | Visible | Visible | Hidden |

As of v3.2.0, the `.visible-*-*` classes for each breakpoint come in three variations, one for each CSS display property value listed below.

Group of classes | CSS `display| `
|----|----|
| `.visible-*-block` | `display: block;| `
| `.visible-*-inline` | `display: inline;| `
| `.visible-*-inline-block` | `display: inline-block;| `

So, for extra small (xs) screens for example, the available `.visible-*-*` classes are: `.visible-xs-block`, `.visible-xs-inline`, and `.visible-xs-inline-block`.

The classes `.visible-xs`, `.visible-sm`, `.visible-md`, and `.visible-lg` also exist, but are **deprecated as of v3.2.0**. They are approximately equivalent to `.visible-*-block`, except with additional special cases for toggling `<table>`-related elements.

#### Print classes

Similar to the regular responsive classes, use these for toggling content for print.
| Classes | Browser | Print |
|----|----|----|
| `.visible-print-block`, `.visible-print-inline`, `.visible-print-inline-block` | Hidden | Visible |
| `.hidden-print` | Visible | Hidden |

The class `.visible-print` also exists but is **deprecated** as of v3.2.0. It is approximately equivalent to `.visible-print-block`, except with additional special cases for `<table>`-related elements.

#### Test cases

Resize your browser or load on different devices to test the responsive utility classes.

##### Visible on...

Green checkmarks indicate the element is visible in your current viewport.

![IMG](IMG)

#### Hidden on...

Here, green checkmarks also indicate the element is hidden in your current viewport.

![IMG](IMG)

### Using Less

**Bootstrap's CSS is built on Less, a preprocessor with additional functionality like variables, mixins, and functions for compiling CSS. Those looking to use the source Less files instead of our compiled CSS files can make use of the numerous variables and mixins we use throughout the framework.**

Grid variables and mixins are covered [within the Grid system section](https://getbootstrap.com/docs/3.3/css/#grid-less).

#### Compiling Bootstrap

Bootstrap can be used in at least two ways: with the compiled CSS or with the source Less files. To compile the Less files, [consult the Getting Started section](https://getbootstrap.com/docs/3.3/getting-started/#grunt) for how to setup your development environment to run the necessary commands.

Third party compilation tools may work with Bootstrap, but they are not supported by our core team.

#### Variables

Variables are used throughout the entire project as a way to centralize and share commonly used values like colors, spacing, or font stacks. For a complete breakdown, please see [the Customizer](https://getbootstrap.com/docs/3.3/customize/#less-variables-section).

##### Colors

Easily make use of two color schemes: grayscale and semantic. Grayscale colors provide quick access to commonly used shades of black while semantic include various colors assigned to meaningful contextual values.

![IMG](IMG)

    ```less
    @gray-darker:  lighten(#000, 13.5%); // #222
    @gray-dark:    lighten(#000, 20%);   // #333
    @gray:         lighten(#000, 33.5%); // #555
    @gray-light:   lighten(#000, 46.7%); // #777
    @gray-lighter: lighten(#000, 93.5%); // #eee
    ```

![IMG](IMG)

    ```less
    @brand-primary: darken(#428bca, 6.5%); // #337ab7
    @brand-success: #5cb85c;
    @brand-info:    #5bc0de;
    @brand-warning: #f0ad4e;
    @brand-danger:  #d9534f;
```

Use any of these color variables as they are or reassign them to more meaningful variables for your project.

    ```less
    // Use as-is
    .masthead {
      background-color: @brand-primary;
    }
    // Reassigned variables in Less
    @alert-message-background: @brand-info;
    .alert {
      background-color: @alert-message-background;
    }
    ```

##### Scaffolding

A handful of variables for quickly customizing key elements of your site's skeleton.

    ```less
    // Scaffolding
    @body-bg:    #fff;
    @text-color: @black-50;
    ```

##### Links

Easily style your links with the right color with only one value.

    ```less
    // Variables
    @link-color:       @brand-primary;
    @link-hover-color: darken(@link-color, 15%);
    // Usage
    a {
      color: @link-color;
      text-decoration: none;
      &:hover {
        color: @link-hover-color;
        text-decoration: underline;
      }
    }
    ```

Note that the `@link-hover-color` uses a function, another awesome tool from Less, to automagically create the right hover color. You can use `darken`, `lighten`, `saturate`, and `desaturate`.

##### Typography

Easily set your typeface, text size, leading, and more with a few quick variables. Bootstrap makes use of these as well to provide easy typographic mixins.

    ```less
    @font-family-sans-serif:  "Helvetica Neue", Helvetica, Arial, sans-serif;
    @font-family-serif:       Georgia, "Times New Roman", Times, serif;
    @font-family-monospace:   Menlo, Monaco, Consolas, "Courier New", monospace;
    @font-family-base:        @font-family-sans-serif;
    @font-size-base:          14px;
    @font-size-large:         ceil((@font-size-base * 1.25)); // ~18px
    @font-size-small:         ceil((@font-size-base * 0.85)); // ~12px
    @font-size-h1:            floor((@font-size-base * 2.6)); // ~36px
    @font-size-h2:            floor((@font-size-base * 2.15)); // ~30px
    @font-size-h3:            ceil((@font-size-base * 1.7)); // ~24px
    @font-size-h4:            ceil((@font-size-base * 1.25)); // ~18px
    @font-size-h5:            @font-size-base;
    @font-size-h6:            ceil((@font-size-base * 0.85)); // ~12px
    @line-height-base:        1.428571429; // 20/14
    @line-height-computed:    floor((@font-size-base * @line-height-base)); // ~20px
    @headings-font-family:    inherit;
    @headings-font-weight:    500;
    @headings-line-height:    1.1;
    @headings-color:          inherit;
    ```

##### Icons

Two quick variables for customizing the location and filename of your icons.

    ```less
    @icon-font-path:          "../fonts/";
    @icon-font-name:          "glyphicons-halflings-regular";
    ```

##### Components

Components throughout Bootstrap make use of some default variables for setting common values. Here are the most commonly used.

    ```less
    @padding-base-vertical:          6px;
    @padding-base-horizontal:        12px;
    @padding-large-vertical:         10px;
    @padding-large-horizontal:       16px;
    @padding-small-vertical:         5px;
    @padding-small-horizontal:       10px;
    @padding-xs-vertical:            1px;
    @padding-xs-horizontal:          5px;
    @line-height-large:              1.33;
    @line-height-small:              1.5;
    @border-radius-base:             4px;
    @border-radius-large:            6px;
    @border-radius-small:            3px;
    @component-active-color:         #fff;
    @component-active-bg:            @brand-primary;
    @caret-width-base:               4px;
    @caret-width-large:              5px;
    ```

#### Vendor mixins

Vendor mixins are mixins to help support multiple browsers by including all relevant vendor prefixes in your compiled CSS.

##### Box-sizing

Reset your components' box model with a single mixin. For context, see this [helpful article from Mozilla](https://developer.mozilla.org/en-US/docs/CSS/box-sizing).

The mixin is **deprecated** as of v3.2.0, with the introduction of Autoprefixer. To preserve backwards-compatibility, Bootstrap will continue to use the mixin internally until Bootstrap v4.

    ```less
    .box-sizing(@box-model) {
      -webkit-box-sizing: @box-model; // Safari <= 5
         -moz-box-sizing: @box-model; // Firefox <= 19
              box-sizing: @box-model;
    }
    ```

##### Rounded corners

Today all modern browsers support the non-prefixed `border-radius` property. As such, there is no `.border-radius()` mixin, but Bootstrap does include shortcuts for quickly rounding two corners on a particular side of an object.

    ```less
    .border-top-radius(@radius) {
      border-top-right-radius: @radius;
       border-top-left-radius: @radius;
    }
    .border-right-radius(@radius) {
      border-bottom-right-radius: @radius;
         border-top-right-radius: @radius;
    }
    .border-bottom-radius(@radius) {
      border-bottom-right-radius: @radius;
       border-bottom-left-radius: @radius;
    }
    .border-left-radius(@radius) {
      border-bottom-left-radius: @radius;
         border-top-left-radius: @radius;
    }
    ```

##### Box (Drop) shadows

If your target audience is using the latest and greatest browsers and devices, be sure to just use the box-shadow property on its own. If you need support for older Android (pre-v4) and iOS devices (pre-iOS 5), use the **deprecated** mixin to pick up the required `-webkit` prefix.

The mixin is **deprecated** as of v3.1.0, since Bootstrap doesn't officially support the outdated platforms that don't support the standard property. To preserve backwards-compatibility, Bootstrap will continue to use the mixin internally until Bootstrap v4.

Be sure to use `rgba()` colors in your box shadows so they blend as seamlessly as possible with backgrounds.

    ```less
    .box-shadow(@shadow: 0 1px 3px rgba(0,0,0,.25)) {
      -webkit-box-shadow: @shadow; // iOS <4.3 & Android <4.1
              box-shadow: @shadow;
    }
    ```

##### Transitions

Multiple mixins for flexibility. Set all transition information with one, or specify a separate delay and duration as needed.

The mixins are **deprecated** as of v3.2.0, with the introduction of Autoprefixer. To preserve backwards-compatibility, Bootstrap will continue to use the mixins internally until Bootstrap v4.

    ```less
    .transition(@transition) {
      -webkit-transition: @transition;
              transition: @transition;
    }
    .transition-property(@transition-property) {
      -webkit-transition-property: @transition-property;
              transition-property: @transition-property;
    }
    .transition-delay(@transition-delay) {
      -webkit-transition-delay: @transition-delay;
              transition-delay: @transition-delay;
    }
    .transition-duration(@transition-duration) {
      -webkit-transition-duration: @transition-duration;
              transition-duration: @transition-duration;
    }
    .transition-timing-function(@timing-function) {
      -webkit-transition-timing-function: @timing-function;
              transition-timing-function: @timing-function;
    }
    .transition-transform(@transition) {
      -webkit-transition: -webkit-transform @transition;
         -moz-transition: -moz-transform @transition;
           -o-transition: -o-transform @transition;
              transition: transform @transition;
    }
    ```

##### Transformations

Rotate, scale, translate (move), or skew any object.

The mixins are **deprecated** as of v3.2.0, with the introduction of Autoprefixer. To preserve backwards-compatibility, Bootstrap will continue to use the mixins internally until Bootstrap v4.

    ```less
    .rotate(@degrees) {
      -webkit-transform: rotate(@degrees);
          -ms-transform: rotate(@degrees); // IE9 only
              transform: rotate(@degrees);
    }
    .scale(@ratio; @ratio-y...) {
      -webkit-transform: scale(@ratio, @ratio-y);
          -ms-transform: scale(@ratio, @ratio-y); // IE9 only
              transform: scale(@ratio, @ratio-y);
    }
    .translate(@x; @y) {
      -webkit-transform: translate(@x, @y);
          -ms-transform: translate(@x, @y); // IE9 only
              transform: translate(@x, @y);
    }
    .skew(@x; @y) {
      -webkit-transform: skew(@x, @y);
          -ms-transform: skewX(@x) skewY(@y); // See https://github.com/twbs/bootstrap/issues/4885; IE9+
              transform: skew(@x, @y);
    }
    .translate3d(@x; @y; @z) {
      -webkit-transform: translate3d(@x, @y, @z);
              transform: translate3d(@x, @y, @z);
    }
    .rotateX(@degrees) {
      -webkit-transform: rotateX(@degrees);
          -ms-transform: rotateX(@degrees); // IE9 only
              transform: rotateX(@degrees);
    }
    .rotateY(@degrees) {
      -webkit-transform: rotateY(@degrees);
          -ms-transform: rotateY(@degrees); // IE9 only
              transform: rotateY(@degrees);
    }
    .perspective(@perspective) {
      -webkit-perspective: @perspective;
         -moz-perspective: @perspective;
              perspective: @perspective;
    }
    .perspective-origin(@perspective) {
      -webkit-perspective-origin: @perspective;
         -moz-perspective-origin: @perspective;
              perspective-origin: @perspective;
    }
    .transform-origin(@origin) {
      -webkit-transform-origin: @origin;
         -moz-transform-origin: @origin;
          -ms-transform-origin: @origin; // IE9 only
              transform-origin: @origin;
    }
    ```

##### Animations

A single mixin for using all of CSS3's animation properties in one declaration and other mixins for individual properties.

The mixins are **deprecated** as of v3.2.0, with the introduction of Autoprefixer. To preserve backwards-compatibility, Bootstrap will continue to use the mixins internally until Bootstrap v4.

    ```less
    .animation(@animation) {
      -webkit-animation: @animation;
              animation: @animation;
    }
    .animation-name(@name) {
      -webkit-animation-name: @name;
              animation-name: @name;
    }
    .animation-duration(@duration) {
      -webkit-animation-duration: @duration;
              animation-duration: @duration;
    }
    .animation-timing-function(@timing-function) {
      -webkit-animation-timing-function: @timing-function;
              animation-timing-function: @timing-function;
    }
    .animation-delay(@delay) {
      -webkit-animation-delay: @delay;
              animation-delay: @delay;
    }
    .animation-iteration-count(@iteration-count) {
      -webkit-animation-iteration-count: @iteration-count;
              animation-iteration-count: @iteration-count;
    }
    .animation-direction(@direction) {
      -webkit-animation-direction: @direction;
              animation-direction: @direction;
    }
    ```

##### Opacity

Set the opacity for all browsers and provide a `filter` fallback for IE8.

    ```less
    .opacity(@opacity) {
      opacity: @opacity;
      // IE8 filter
      @opacity-ie: (@opacity * 100);
      filter: ~"alpha(opacity=@{opacity-ie})";
    }
    ```

##### Placeholder text

Provide context for form controls within each field.

    ```less
    .placeholder(@color: @input-color-placeholder) {
      &::-moz-placeholder           { color: @color; } // Firefox
      &:-ms-input-placeholder       { color: @color; } // Internet Explorer 10+
      &::-webkit-input-placeholder  { color: @color; } // Safari and Chrome
    }
    ```

##### Columns

Generate columns via CSS within a single element.

    ```less
    .content-columns(@width; @count; @gap) {
      -webkit-column-width: @width;
         -moz-column-width: @width;
              column-width: @width;
      -webkit-column-count: @count;
         -moz-column-count: @count;
              column-count: @count;
      -webkit-column-gap: @gap;
         -moz-column-gap: @gap;
              column-gap: @gap;
    }
    ```

##### Gradients

Easily turn any two colors into a background gradient. Get more advanced and set a direction, use three colors, or use a radial gradient. With a single mixin you get all the prefixed syntaxes you'll need.

    ```less
    #gradient > .vertical(#333; #000);
    #gradient > .horizontal(#333; #000);
    #gradient > .radial(#333; #000);
    ```

You can also specify the angle of a standard two-color, linear gradient:

    ```less
    #gradient > .directional(#333; #000; 45deg);
    ```

If you need a barber-stripe style gradient, that's easy, too. Just specify a single color and we'll overlay a translucent white stripe.

    ```less
    #gradient > .striped(#333; 45deg);
    ```

Up the ante and use three colors instead. Set the first color, the second color, the second color's color stop (a percentage value like 25%), and the third color with these mixins:

    ```less
    #gradient > .vertical-three-colors(#777; #333; 25%; #000);
    #gradient > .horizontal-three-colors(#777; #333; 25%; #000);
    ```

**Heads up!** Should you ever need to remove a gradient, be sure to remove any IE-specific `filter` you may have added. You can do that by using the `.reset-filter()` mixin alongside `background-image: none;`.

#### Utility mixins

Utility mixins are mixins that combine otherwise unrelated CSS properties to achieve a specific goal or task.

##### Clearfix

Forget adding class="clearfix" to any element and instead add the .clearfix() mixin where appropriate. Uses the micro clearfix from Nicolas Gallagher.

    ```less
    // Mixin
    .clearfix() {
      &:before,
      &:after {
        content: " ";
        display: table;
      }
      &:after {
        clear: both;
      }
    }
    // Usage
    .container {
      .clearfix();
    }
    ```

##### Horizontal centering

Quickly center any element within its parent. Requires width or max-width to be set.

    ```less
    // Mixin
    .center-block() {
      display: block;
      margin-left: auto;
      margin-right: auto;
    }
    // Usage
    .container {
      width: 940px;
      .center-block();
    }
    ```

##### Sizing helpers

Specify the dimensions of an object more easily.

    ```less
    // Mixins
    .size(@width; @height) {
      width: @width;
      height: @height;
    }
    .square(@size) {
      .size(@size; @size);
    }
    // Usage
    .image { .size(400px; 300px); }
    .avatar { .square(48px); }
    ```

##### Resizable textareas

Easily configure the resize options for any textarea, or any other element. Defaults to normal browser behavior (`both`).

    ```less
    .resizable(@direction: both) {
      // Options: horizontal, vertical, both
      resize: @direction;
      // Safari fix
      overflow: auto;
    }
    ```

##### Truncating text

**Easily truncate text with an ellipsis with a single mixin. Requires element to be `block` or `inline-block` level.**

    ```less
    // Mixin
    .text-overflow() {
      overflow: hidden;
      text-overflow: ellipsis;
      white-space: nowrap;
    }
    // Usage
    .branch-name {
      display: inline-block;
      max-width: 200px;
      .text-overflow();
    }
    ```

##### Retina images

Specify two image paths and the @1x image dimensions, and Bootstrap will provide an @2x media query. **If you have many images to serve, consider writing your retina image CSS manually in a single media query.**

    ```less
    .img-retina(@file-1x; @file-2x; @width-1x; @height-1x) {
      background-image: url("@{file-1x}");

      @media
      only screen and (-webkit-min-device-pixel-ratio: 2),
      only screen and (   min--moz-device-pixel-ratio: 2),
      only screen and (     -o-min-device-pixel-ratio: 2/1),
      only screen and (        min-device-pixel-ratio: 2),
      only screen and (                min-resolution: 192dpi),
      only screen and (                min-resolution: 2dppx) {
        background-image: url("@{file-2x}");
        background-size: @width-1x @height-1x;
      }
    }
    // Usage
    .jumbotron {
      .img-retina("/img/bg-1x.png", "/img/bg-2x.png", 100px, 100px);
    }
    ```

### Using Sass

**While Bootstrap is built on Less, it also has an [official Sass port](https://github.com/twbs/bootstrap-sass). We maintain it in a separate GitHub repository and handle updates with a conversion script.**

#### What's included

Since the Sass port has a separate repo and serves a slightly different audience, the contents of the project differ greatly from the main Bootstrap project. This ensures the Sass port is as compatible with as many Sass-based systems as possible.

| Path | Description |
|-----|-----|
| `lib/` | Ruby gem code (Sass configuration, Rails and Compass integrations) | 
| `tasks/` | Converter scripts (turning upstream Less to Sass) | 
| `test/` | Compilation tests | 
| `templates/` | Compass package manifest | 
| `vendor/assets/` | Sass, JavaScript, and font files |
| `Rakefile` | Internal tasks, such as rake and convert |

Visit the Sass port's GitHub repository to see these files in action.

#### Installation

For information on how to install and use Bootstrap for Sass, consult the [GitHub repository readme](https://github.com/twbs/bootstrap-sass). It's the most up to date source and includes information for use with Rails, Compass, and standard Sass projects.

[Bootstrap for Sass](https://github.com/twbs/bootstrap-sass)

-------------------------------------------------------------------------------

## Components

Over a dozen reusable components built to provide iconography, dropdowns, input groups, navigation, alerts, and much more.
Glyphicons
Available glyphs

Includes over 250 glyphs in font format from the Glyphicon Halflings set. Glyphicons Halflings are normally not available for free, but their creator has made them available for Bootstrap free of cost. As a thank you, we only ask that you include a link back to Glyphicons whenever possible.

    glyphicon glyphicon-asterisk
    glyphicon glyphicon-plus
    glyphicon glyphicon-euro
    glyphicon glyphicon-eur
    glyphicon glyphicon-minus
    glyphicon glyphicon-cloud
    glyphicon glyphicon-envelope
    glyphicon glyphicon-pencil
    glyphicon glyphicon-glass
    glyphicon glyphicon-music
    glyphicon glyphicon-search
    glyphicon glyphicon-heart
    glyphicon glyphicon-star
    glyphicon glyphicon-star-empty
    glyphicon glyphicon-user
    glyphicon glyphicon-film
    glyphicon glyphicon-th-large
    glyphicon glyphicon-th
    glyphicon glyphicon-th-list
    glyphicon glyphicon-ok
    glyphicon glyphicon-remove
    glyphicon glyphicon-zoom-in
    glyphicon glyphicon-zoom-out
    glyphicon glyphicon-off
    glyphicon glyphicon-signal
    glyphicon glyphicon-cog
    glyphicon glyphicon-trash
    glyphicon glyphicon-home
    glyphicon glyphicon-file
    glyphicon glyphicon-time
    glyphicon glyphicon-road
    glyphicon glyphicon-download-alt
    glyphicon glyphicon-download
    glyphicon glyphicon-upload
    glyphicon glyphicon-inbox
    glyphicon glyphicon-play-circle
    glyphicon glyphicon-repeat
    glyphicon glyphicon-refresh
    glyphicon glyphicon-list-alt
    glyphicon glyphicon-lock
    glyphicon glyphicon-flag
    glyphicon glyphicon-headphones
    glyphicon glyphicon-volume-off
    glyphicon glyphicon-volume-down
    glyphicon glyphicon-volume-up
    glyphicon glyphicon-qrcode
    glyphicon glyphicon-barcode
    glyphicon glyphicon-tag
    glyphicon glyphicon-tags
    glyphicon glyphicon-book
    glyphicon glyphicon-bookmark
    glyphicon glyphicon-print
    glyphicon glyphicon-camera
    glyphicon glyphicon-font
    glyphicon glyphicon-bold
    glyphicon glyphicon-italic
    glyphicon glyphicon-text-height
    glyphicon glyphicon-text-width
    glyphicon glyphicon-align-left
    glyphicon glyphicon-align-center
    glyphicon glyphicon-align-right
    glyphicon glyphicon-align-justify
    glyphicon glyphicon-list
    glyphicon glyphicon-indent-left
    glyphicon glyphicon-indent-right
    glyphicon glyphicon-facetime-video
    glyphicon glyphicon-picture
    glyphicon glyphicon-map-marker
    glyphicon glyphicon-adjust
    glyphicon glyphicon-tint
    glyphicon glyphicon-edit
    glyphicon glyphicon-share
    glyphicon glyphicon-check
    glyphicon glyphicon-move
    glyphicon glyphicon-step-backward
    glyphicon glyphicon-fast-backward
    glyphicon glyphicon-backward
    glyphicon glyphicon-play
    glyphicon glyphicon-pause
    glyphicon glyphicon-stop
    glyphicon glyphicon-forward
    glyphicon glyphicon-fast-forward
    glyphicon glyphicon-step-forward
    glyphicon glyphicon-eject
    glyphicon glyphicon-chevron-left
    glyphicon glyphicon-chevron-right
    glyphicon glyphicon-plus-sign
    glyphicon glyphicon-minus-sign
    glyphicon glyphicon-remove-sign
    glyphicon glyphicon-ok-sign
    glyphicon glyphicon-question-sign
    glyphicon glyphicon-info-sign
    glyphicon glyphicon-screenshot
    glyphicon glyphicon-remove-circle
    glyphicon glyphicon-ok-circle
    glyphicon glyphicon-ban-circle
    glyphicon glyphicon-arrow-left
    glyphicon glyphicon-arrow-right
    glyphicon glyphicon-arrow-up
    glyphicon glyphicon-arrow-down
    glyphicon glyphicon-share-alt
    glyphicon glyphicon-resize-full
    glyphicon glyphicon-resize-small
    glyphicon glyphicon-exclamation-sign
    glyphicon glyphicon-gift
    glyphicon glyphicon-leaf
    glyphicon glyphicon-fire
    glyphicon glyphicon-eye-open
    glyphicon glyphicon-eye-close
    glyphicon glyphicon-warning-sign
    glyphicon glyphicon-plane
    glyphicon glyphicon-calendar
    glyphicon glyphicon-random
    glyphicon glyphicon-comment
    glyphicon glyphicon-magnet
    glyphicon glyphicon-chevron-up
    glyphicon glyphicon-chevron-down
    glyphicon glyphicon-retweet
    glyphicon glyphicon-shopping-cart
    glyphicon glyphicon-folder-close
    glyphicon glyphicon-folder-open
    glyphicon glyphicon-resize-vertical
    glyphicon glyphicon-resize-horizontal
    glyphicon glyphicon-hdd
    glyphicon glyphicon-bullhorn
    glyphicon glyphicon-bell
    glyphicon glyphicon-certificate
    glyphicon glyphicon-thumbs-up
    glyphicon glyphicon-thumbs-down
    glyphicon glyphicon-hand-right
    glyphicon glyphicon-hand-left
    glyphicon glyphicon-hand-up
    glyphicon glyphicon-hand-down
    glyphicon glyphicon-circle-arrow-right
    glyphicon glyphicon-circle-arrow-left
    glyphicon glyphicon-circle-arrow-up
    glyphicon glyphicon-circle-arrow-down
    glyphicon glyphicon-globe
    glyphicon glyphicon-wrench
    glyphicon glyphicon-tasks
    glyphicon glyphicon-filter
    glyphicon glyphicon-briefcase
    glyphicon glyphicon-fullscreen
    glyphicon glyphicon-dashboard
    glyphicon glyphicon-paperclip
    glyphicon glyphicon-heart-empty
    glyphicon glyphicon-link
    glyphicon glyphicon-phone
    glyphicon glyphicon-pushpin
    glyphicon glyphicon-usd
    glyphicon glyphicon-gbp
    glyphicon glyphicon-sort
    glyphicon glyphicon-sort-by-alphabet
    glyphicon glyphicon-sort-by-alphabet-alt
    glyphicon glyphicon-sort-by-order
    glyphicon glyphicon-sort-by-order-alt
    glyphicon glyphicon-sort-by-attributes
    glyphicon glyphicon-sort-by-attributes-alt
    glyphicon glyphicon-unchecked
    glyphicon glyphicon-expand
    glyphicon glyphicon-collapse-down
    glyphicon glyphicon-collapse-up
    glyphicon glyphicon-log-in
    glyphicon glyphicon-flash
    glyphicon glyphicon-log-out
    glyphicon glyphicon-new-window
    glyphicon glyphicon-record
    glyphicon glyphicon-save
    glyphicon glyphicon-open
    glyphicon glyphicon-saved
    glyphicon glyphicon-import
    glyphicon glyphicon-export
    glyphicon glyphicon-send
    glyphicon glyphicon-floppy-disk
    glyphicon glyphicon-floppy-saved
    glyphicon glyphicon-floppy-remove
    glyphicon glyphicon-floppy-save
    glyphicon glyphicon-floppy-open
    glyphicon glyphicon-credit-card
    glyphicon glyphicon-transfer
    glyphicon glyphicon-cutlery
    glyphicon glyphicon-header
    glyphicon glyphicon-compressed
    glyphicon glyphicon-earphone
    glyphicon glyphicon-phone-alt
    glyphicon glyphicon-tower
    glyphicon glyphicon-stats
    glyphicon glyphicon-sd-video
    glyphicon glyphicon-hd-video
    glyphicon glyphicon-subtitles
    glyphicon glyphicon-sound-stereo
    glyphicon glyphicon-sound-dolby
    glyphicon glyphicon-sound-5-1
    glyphicon glyphicon-sound-6-1
    glyphicon glyphicon-sound-7-1
    glyphicon glyphicon-right-mark
    glyphicon glyphicon-registration-mark
    glyphicon glyphicon-cloud-download
    glyphicon glyphicon-cloud-upload
    glyphicon glyphicon-tree-conifer
    glyphicon glyphicon-tree-deciduous
    glyphicon glyphicon-cd
    glyphicon glyphicon-save-file
    glyphicon glyphicon-open-file
    glyphicon glyphicon-level-up
    glyphicon glyphicon-
    glyphicon glyphicon-paste
    glyphicon glyphicon-alert
    glyphicon glyphicon-equalizer
    glyphicon glyphicon-king
    glyphicon glyphicon-queen
    glyphicon glyphicon-pawn
    glyphicon glyphicon-bishop
    glyphicon glyphicon-knight
    glyphicon glyphicon-baby-formula
    glyphicon glyphicon-tent
    glyphicon glyphicon-blackboard
    glyphicon glyphicon-bed
    glyphicon glyphicon-apple
    glyphicon glyphicon-erase
    glyphicon glyphicon-hourglass
    glyphicon glyphicon-lamp
    glyphicon glyphicon-duplicate
    glyphicon glyphicon-piggy-bank
    glyphicon glyphicon-scissors
    glyphicon glyphicon-bitcoin
    glyphicon glyphicon-btc
    glyphicon glyphicon-xbt
    glyphicon glyphicon-yen
    glyphicon glyphicon-jpy
    glyphicon glyphicon-ruble
    glyphicon glyphicon-rub
    glyphicon glyphicon-scale
    glyphicon glyphicon-ice-lolly
    glyphicon glyphicon-ice-lolly-tasted
    glyphicon glyphicon-education
    glyphicon glyphicon-option-horizontal
    glyphicon glyphicon-option-vertical
    glyphicon glyphicon-menu-hamburger
    glyphicon glyphicon-modal-window
    glyphicon glyphicon-oil
    glyphicon glyphicon-grain
    glyphicon glyphicon-sunglasses
    glyphicon glyphicon-text-size
    glyphicon glyphicon-text-color
    glyphicon glyphicon-text-background
    glyphicon glyphicon-object-align-top
    glyphicon glyphicon-object-align-bottom
    glyphicon glyphicon-object-align-horizontal
    glyphicon glyphicon-object-align-left
    glyphicon glyphicon-object-align-vertical
    glyphicon glyphicon-object-align-right
    glyphicon glyphicon-triangle-right
    glyphicon glyphicon-triangle-left
    glyphicon glyphicon-triangle-bottom
    glyphicon glyphicon-triangle-top
    glyphicon glyphicon-console
    glyphicon glyphicon-superscript
    glyphicon glyphicon-subscript
    glyphicon glyphicon-menu-left
    glyphicon glyphicon-menu-right
    glyphicon glyphicon-menu-down
    glyphicon glyphicon-menu-up

How to use

For performance reasons, all icons require a base class and individual icon class. To use, place the following code just about anywhere. Be sure to leave a space between the icon and text for proper padding.
Don't mix with other components

Icon classes cannot be directly combined with other components. They should not be used along with other classes on the same element. Instead, add a nested <span> and apply the icon classes to the <span>.
Only for use on empty elements

Icon classes should only be used on elements that contain no text content and have no child elements.
Changing the icon font location

Bootstrap assumes icon font files will be located in the ../fonts/ directory, relative to the compiled CSS files. Moving or renaming those font files means updating the CSS in one of three ways:

    Change the @icon-font-path and/or @icon-font-name variables in the source Less files.
    Utilize the relative URLs option provided by the Less compiler.
    Change the url() paths in the compiled CSS.

Use whatever option best suits your specific development setup.
Accessible icons

Modern versions of assistive technologies will announce CSS generated content, as well as specific Unicode characters. To avoid unintended and confusing output in screen readers (particularly when icons are used purely for decoration), we hide them with the aria-hidden="true" attribute.

If you're using an icon to convey meaning (rather than only as a decorative element), ensure that this meaning is also conveyed to assistive technologies – for instance, include additional content, visually hidden with the .sr-only class.

If you're creating controls with no other text (such as a <button> that only contains an icon), you should always provide alternative content to identify the purpose of the control, so that it will make sense to users of assistive technologies. In this case, you could add an aria-label attribute on the control itself.


<span class="glyphicon glyphicon-search" aria-hidden="true"></span>

Examples

Use them in buttons, button groups for a toolbar, navigation, or prepended form inputs.


<button type="button" class="btn btn-default" aria-label="Left Align">
  <span class="glyphicon glyphicon-align-left" aria-hidden="true"></span>
</button>

<button type="button" class="btn btn-default btn-lg">
  <span class="glyphicon glyphicon-star" aria-hidden="true"></span> Star
</button>

An icon used in an alert to convey that it's an error message, with additional .sr-only text to convey this hint to users of assistive technologies.
Error: Enter a valid email address


<div class="alert alert-danger" role="alert">
  <span class="glyphicon glyphicon-exclamation-sign" aria-hidden="true"></span>
  <span class="sr-only">Error:</span>
  Enter a valid email address
</div>

Dropdowns

Toggleable, contextual menu for displaying lists of links. Made interactive with the dropdown JavaScript plugin.
Example

Wrap the dropdown's trigger and the dropdown menu within .dropdown, or another element that declares position: relative;. Then add the menu's HTML.

    Action
    Another action
    Something else here



<div class="dropdown">
  <button class="btn btn-default dropdown-toggle" type="button" id="dropdownMenu1" data-toggle="dropdown" aria-haspopup="true" aria-expanded="true">
    Dropdown
    <span class="caret"></span>
  </button>
  <ul class="dropdown-menu" aria-labelledby="dropdownMenu1">
    <li><a href="#">Action</a></li>
    <li><a href="#">Another action</a></li>
    <li><a href="#">Something else here</a></li>
    <li role="separator" class="divider"></li>
    <li><a href="#">Separated link</a></li>
  </ul>
</div>

Dropdown menus can be changed to expand upwards (instead of downwards) by adding .dropup to the parent.


<div class="dropup">
  <button class="btn btn-default dropdown-toggle" type="button" id="dropdownMenu2" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
    Dropup
    <span class="caret"></span>
  </button>
  <ul class="dropdown-menu" aria-labelledby="dropdownMenu2">
    <li><a href="#">Action</a></li>
    <li><a href="#">Another action</a></li>
    <li><a href="#">Something else here</a></li>
    <li role="separator" class="divider"></li>
    <li><a href="#">Separated link</a></li>
  </ul>
</div>

Alignment

By default, a dropdown menu is automatically positioned 100% from the top and along the left side of its parent. Add .dropdown-menu-right to a .dropdown-menu to right align the dropdown menu.
May require additional positioning

Dropdowns are automatically positioned via CSS within the normal flow of the document. This means dropdowns may be cropped by parents with certain overflow properties or appear out of bounds of the viewport. Address these issues on your own as they arise.
Deprecated .pull-right alignment

As of v3.1.0, we've deprecated .pull-right on dropdown menus. To right-align a menu, use .dropdown-menu-right. Right-aligned nav components in the navbar use a mixin version of this class to automatically align the menu. To override it, use .dropdown-menu-left.


<ul class="dropdown-menu dropdown-menu-right" aria-labelledby="dLabel">
  ...
</ul>

Headers

Add a header to label sections of actions in any dropdown menu.

    Dropdown header
    Action
    Another action
    Something else here
    Dropdown header
    Separated link



<ul class="dropdown-menu" aria-labelledby="dropdownMenu3">
  ...
  <li class="dropdown-header">Dropdown header</li>
  ...
</ul>

Divider

Add a divider to separate series of links in a dropdown menu.

    Action
    Another action
    Something else here
    Separated link



<ul class="dropdown-menu" aria-labelledby="dropdownMenuDivider">
  ...
  <li role="separator" class="divider"></li>
  ...
</ul>

Disabled menu items

Add .disabled to a <li> in the dropdown to disable the link.

    Regular link
    Disabled link
    Another link



<ul class="dropdown-menu" aria-labelledby="dropdownMenu4">
  <li><a href="#">Regular link</a></li>
  <li class="disabled"><a href="#">Disabled link</a></li>
  <li><a href="#">Another link</a></li>
</ul>

Button groups

Group a series of buttons together on a single line with the button group. Add on optional JavaScript radio and checkbox style behavior with our buttons plugin.
Tooltips & popovers in button groups require special setting

When using tooltips or popovers on elements within a .btn-group, you'll have to specify the option container: 'body' to avoid unwanted side effects (such as the element growing wider and/or losing its rounded corners when the tooltip or popover is triggered).
Ensure correct role and provide a label

In order for assistive technologies – such as screen readers – to convey that a series of buttons is grouped, an appropriate role attribute needs to be provided. For button groups, this would be role="group", while toolbars should have a role="toolbar".

One exception are groups which only contain a single control (for instance the justified button groups with <button> elements) or a dropdown.

In addition, groups and toolbars should be given an explicit label, as most assistive technologies will otherwise not announce them, despite the presence of the correct role attribute. In the examples provided here, we use aria-label, but alternatives such as aria-labelledby can also be used.
Basic example

Wrap a series of buttons with .btn in .btn-group.


<div class="btn-group" role="group" aria-label="...">
  <button type="button" class="btn btn-default">Left</button>
  <button type="button" class="btn btn-default">Middle</button>
  <button type="button" class="btn btn-default">Right</button>
</div>

Button toolbar

Combine sets of <div class="btn-group"> into a <div class="btn-toolbar"> for more complex components.


<div class="btn-toolbar" role="toolbar" aria-label="...">
  <div class="btn-group" role="group" aria-label="...">...</div>
  <div class="btn-group" role="group" aria-label="...">...</div>
  <div class="btn-group" role="group" aria-label="...">...</div>
</div>

Sizing

Instead of applying button sizing classes to every button in a group, just add .btn-group-* to each .btn-group, including when nesting multiple groups.





<div class="btn-group btn-group-lg" role="group" aria-label="...">...</div>
<div class="btn-group" role="group" aria-label="...">...</div>
<div class="btn-group btn-group-sm" role="group" aria-label="...">...</div>
<div class="btn-group btn-group-xs" role="group" aria-label="...">...</div>

Nesting

Place a .btn-group within another .btn-group when you want dropdown menus mixed with a series of buttons.


<div class="btn-group" role="group" aria-label="...">
  <button type="button" class="btn btn-default">1</button>
  <button type="button" class="btn btn-default">2</button>

  <div class="btn-group" role="group">
    <button type="button" class="btn btn-default dropdown-toggle" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
      Dropdown
      <span class="caret"></span>
    </button>
    <ul class="dropdown-menu">
      <li><a href="#">Dropdown link</a></li>
      <li><a href="#">Dropdown link</a></li>
    </ul>
  </div>
</div>

Vertical variation

Make a set of buttons appear vertically stacked rather than horizontally. Split button dropdowns are not supported here.


<div class="btn-group-vertical" role="group" aria-label="...">
  ...
</div>

Justified button groups

Make a group of buttons stretch at equal sizes to span the entire width of its parent. Also works with button dropdowns within the button group.
Handling borders

Due to the specific HTML and CSS used to justify buttons (namely display: table-cell), the borders between them are doubled. In regular button groups, margin-left: -1px is used to stack the borders instead of removing them. However, margin doesn't work with display: table-cell. As a result, depending on your customizations to Bootstrap, you may wish to remove or re-color the borders.
IE8 and borders

Internet Explorer 8 doesn't render borders on buttons in a justified button group, whether it's on <a> or <button> elements. To get around that, wrap each button in another .btn-group.

See #12476 for more information.
With <a> elements

Just wrap a series of .btns in .btn-group.btn-group-justified.



<div class="btn-group btn-group-justified" role="group" aria-label="...">
  ...
</div>

Links acting as buttons

If the <a> elements are used to act as buttons – triggering in-page functionality, rather than navigating to another document or section within the current page – they should also be given an appropriate role="button".
With <button> elements

To use justified button groups with <button> elements, you must wrap each button in a button group. Most browsers don't properly apply our CSS for justification to <button> elements, but since we support button dropdowns, we can work around that.


<div class="btn-group btn-group-justified" role="group" aria-label="...">
  <div class="btn-group" role="group">
    <button type="button" class="btn btn-default">Left</button>
  </div>
  <div class="btn-group" role="group">
    <button type="button" class="btn btn-default">Middle</button>
  </div>
  <div class="btn-group" role="group">
    <button type="button" class="btn btn-default">Right</button>
  </div>
</div>

Button dropdowns

Use any button to trigger a dropdown menu by placing it within a .btn-group and providing the proper menu markup.
Plugin dependency

Button dropdowns require the dropdown plugin to be included in your version of Bootstrap.
Single button dropdowns

Turn a button into a dropdown toggle with some basic markup changes.


<!-- Single button -->
<div class="btn-group">
  <button type="button" class="btn btn-default dropdown-toggle" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
    Action <span class="caret"></span>
  </button>
  <ul class="dropdown-menu">
    <li><a href="#">Action</a></li>
    <li><a href="#">Another action</a></li>
    <li><a href="#">Something else here</a></li>
    <li role="separator" class="divider"></li>
    <li><a href="#">Separated link</a></li>
  </ul>
</div>

Split button dropdowns

Similarly, create split button dropdowns with the same markup changes, only with a separate button.


<!-- Split button -->
<div class="btn-group">
  <button type="button" class="btn btn-danger">Action</button>
  <button type="button" class="btn btn-danger dropdown-toggle" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
    <span class="caret"></span>
    <span class="sr-only">Toggle Dropdown</span>
  </button>
  <ul class="dropdown-menu">
    <li><a href="#">Action</a></li>
    <li><a href="#">Another action</a></li>
    <li><a href="#">Something else here</a></li>
    <li role="separator" class="divider"></li>
    <li><a href="#">Separated link</a></li>
  </ul>
</div>

Sizing

Button dropdowns work with buttons of all sizes.


<!-- Large button group -->
<div class="btn-group">
  <button class="btn btn-default btn-lg dropdown-toggle" type="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
    Large button <span class="caret"></span>
  </button>
  <ul class="dropdown-menu">
    ...
  </ul>
</div>

<!-- Small button group -->
<div class="btn-group">
  <button class="btn btn-default btn-sm dropdown-toggle" type="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
    Small button <span class="caret"></span>
  </button>
  <ul class="dropdown-menu">
    ...
  </ul>
</div>

<!-- Extra small button group -->
<div class="btn-group">
  <button class="btn btn-default btn-xs dropdown-toggle" type="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
    Extra small button <span class="caret"></span>
  </button>
  <ul class="dropdown-menu">
    ...
  </ul>
</div>

Dropup variation

Trigger dropdown menus above elements by adding .dropup to the parent.


<div class="btn-group dropup">
  <button type="button" class="btn btn-default">Dropup</button>
  <button type="button" class="btn btn-default dropdown-toggle" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
    <span class="caret"></span>
    <span class="sr-only">Toggle Dropdown</span>
  </button>
  <ul class="dropdown-menu">
    <!-- Dropdown menu links -->
  </ul>
</div>

Input groups

Extend form controls by adding text or buttons before, after, or on both sides of any text-based <input>. Use .input-group with an .input-group-addon or .input-group-btn to prepend or append elements to a single .form-control.
Textual <input>s only

Avoid using <select> elements here as they cannot be fully styled in WebKit browsers.

Avoid using <textarea> elements here as their rows attribute will not be respected in some cases.
Tooltips & popovers in input groups require special setting

When using tooltips or popovers on elements within an .input-group, you'll have to specify the option container: 'body' to avoid unwanted side effects (such as the element growing wider and/or losing its rounded corners when the tooltip or popover is triggered).
Don't mix with other components

Do not mix form groups or grid column classes directly with input groups. Instead, nest the input group inside of the form group or grid-related element.
Always add labels

Screen readers will have trouble with your forms if you don't include a label for every input. For these input groups, ensure that any additional label or functionality is conveyed to assistive technologies.

The exact technique to be used (visible <label> elements, <label> elements hidden using the .sr-only class, or use of the aria-label, aria-labelledby, aria-describedby, title or placeholder attribute) and what additional information will need to be conveyed will vary depending on the exact type of interface widget you're implementing. The examples in this section provide a few suggested, case-specific approaches.
Basic example

Place one add-on or button on either side of an input. You may also place one on both sides of an input.

We do not support multiple add-ons (.input-group-addon or .input-group-btn) on a single side.

We do not support multiple form-controls in a single input group.
@

@example.com

$ .00

Your vanity URL
https://example.com/users/


<div class="input-group">
  <span class="input-group-addon" id="basic-addon1">@</span>
  <input type="text" class="form-control" placeholder="Username" aria-describedby="basic-addon1">
</div>

<div class="input-group">
  <input type="text" class="form-control" placeholder="Recipient's username" aria-describedby="basic-addon2">
  <span class="input-group-addon" id="basic-addon2">@example.com</span>
</div>

<div class="input-group">
  <span class="input-group-addon">$</span>
  <input type="text" class="form-control" aria-label="Amount (to the nearest dollar)">
  <span class="input-group-addon">.00</span>
</div>

<label for="basic-url">Your vanity URL</label>
<div class="input-group">
  <span class="input-group-addon" id="basic-addon3">https://example.com/users/</span>
  <input type="text" class="form-control" id="basic-url" aria-describedby="basic-addon3">
</div>

Sizing

Add the relative form sizing classes to the .input-group itself and contents within will automatically resize—no need for repeating the form control size classes on each element.
@

@

@


<div class="input-group input-group-lg">
  <span class="input-group-addon" id="sizing-addon1">@</span>
  <input type="text" class="form-control" placeholder="Username" aria-describedby="sizing-addon1">
</div>

<div class="input-group">
  <span class="input-group-addon" id="sizing-addon2">@</span>
  <input type="text" class="form-control" placeholder="Username" aria-describedby="sizing-addon2">
</div>

<div class="input-group input-group-sm">
  <span class="input-group-addon" id="sizing-addon3">@</span>
  <input type="text" class="form-control" placeholder="Username" aria-describedby="sizing-addon3">
</div>

Checkboxes and radio addons

Place any checkbox or radio option within an input group's addon instead of text.


<div class="row">
  <div class="col-lg-6">
    <div class="input-group">
      <span class="input-group-addon">
        <input type="checkbox" aria-label="...">
      </span>
      <input type="text" class="form-control" aria-label="...">
    </div><!-- /input-group -->
  </div><!-- /.col-lg-6 -->
  <div class="col-lg-6">
    <div class="input-group">
      <span class="input-group-addon">
        <input type="radio" aria-label="...">
      </span>
      <input type="text" class="form-control" aria-label="...">
    </div><!-- /input-group -->
  </div><!-- /.col-lg-6 -->
</div><!-- /.row -->

Button addons

Buttons in input groups are a bit different and require one extra level of nesting. Instead of .input-group-addon, you'll need to use .input-group-btn to wrap the buttons. This is required due to default browser styles that cannot be overridden.


<div class="row">
  <div class="col-lg-6">
    <div class="input-group">
      <span class="input-group-btn">
        <button class="btn btn-default" type="button">Go!</button>
      </span>
      <input type="text" class="form-control" placeholder="Search for...">
    </div><!-- /input-group -->
  </div><!-- /.col-lg-6 -->
  <div class="col-lg-6">
    <div class="input-group">
      <input type="text" class="form-control" placeholder="Search for...">
      <span class="input-group-btn">
        <button class="btn btn-default" type="button">Go!</button>
      </span>
    </div><!-- /input-group -->
  </div><!-- /.col-lg-6 -->
</div><!-- /.row -->

Buttons with dropdowns


<div class="row">
  <div class="col-lg-6">
    <div class="input-group">
      <div class="input-group-btn">
        <button type="button" class="btn btn-default dropdown-toggle" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">Action <span class="caret"></span></button>
        <ul class="dropdown-menu">
          <li><a href="#">Action</a></li>
          <li><a href="#">Another action</a></li>
          <li><a href="#">Something else here</a></li>
          <li role="separator" class="divider"></li>
          <li><a href="#">Separated link</a></li>
        </ul>
      </div><!-- /btn-group -->
      <input type="text" class="form-control" aria-label="...">
    </div><!-- /input-group -->
  </div><!-- /.col-lg-6 -->
  <div class="col-lg-6">
    <div class="input-group">
      <input type="text" class="form-control" aria-label="...">
      <div class="input-group-btn">
        <button type="button" class="btn btn-default dropdown-toggle" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">Action <span class="caret"></span></button>
        <ul class="dropdown-menu dropdown-menu-right">
          <li><a href="#">Action</a></li>
          <li><a href="#">Another action</a></li>
          <li><a href="#">Something else here</a></li>
          <li role="separator" class="divider"></li>
          <li><a href="#">Separated link</a></li>
        </ul>
      </div><!-- /btn-group -->
    </div><!-- /input-group -->
  </div><!-- /.col-lg-6 -->
</div><!-- /.row -->

Segmented buttons


<div class="input-group">
  <div class="input-group-btn">
    <!-- Button and dropdown menu -->
  </div>
  <input type="text" class="form-control" aria-label="...">
</div>

<div class="input-group">
  <input type="text" class="form-control" aria-label="...">
  <div class="input-group-btn">
    <!-- Button and dropdown menu -->
  </div>
</div>

Multiple buttons

While you can only have one add-on per side, you can have multiple buttons inside a single .input-group-btn.


<div class="input-group">
  <div class="input-group-btn">
    <!-- Buttons -->
  </div>
  <input type="text" class="form-control" aria-label="...">
</div>

<div class="input-group">
  <input type="text" class="form-control" aria-label="...">
  <div class="input-group-btn">
    <!-- Buttons -->
  </div>
</div>

Navs

Navs available in Bootstrap have shared markup, starting with the base .nav class, as well as shared states. Swap modifier classes to switch between each style.
Using navs for tab panels requires JavaScript tabs plugin

For tabs with tabbable areas, you must use the tabs JavaScript plugin. The markup will also require additional role and ARIA attributes – see the plugin's example markup for further details.
Make navs used as navigation accessible

If you are using navs to provide a navigation bar, be sure to add a role="navigation" to the most logical parent container of the <ul>, or wrap a <nav> element around the whole navigation. Do not add the role to the <ul> itself, as this would prevent it from being announced as an actual list by assistive technologies.
Tabs

Note the .nav-tabs class requires the .nav base class.

    Home
    Profile
    Messages



<ul class="nav nav-tabs">
  <li role="presentation" class="active"><a href="#">Home</a></li>
  <li role="presentation"><a href="#">Profile</a></li>
  <li role="presentation"><a href="#">Messages</a></li>
</ul>

Pills

Take that same HTML, but use .nav-pills instead:

    Home
    Profile
    Messages



<ul class="nav nav-pills">
  <li role="presentation" class="active"><a href="#">Home</a></li>
  <li role="presentation"><a href="#">Profile</a></li>
  <li role="presentation"><a href="#">Messages</a></li>
</ul>

Pills are also vertically stackable. Just add .nav-stacked.

    Home
    Profile
    Messages



<ul class="nav nav-pills nav-stacked">
  ...
</ul>

Justified

Easily make tabs or pills equal widths of their parent at screens wider than 768px with .nav-justified. On smaller screens, the nav links are stacked.

Justified navbar nav links are currently not supported.
Safari and responsive justified navs

As of v9.1.2, Safari exhibits a bug in which resizing your browser horizontally causes rendering errors in the justified nav that are cleared upon refreshing. This bug is also shown in the justified nav example.

    Home
    Profile
    Messages


    Home
    Profile
    Messages



<ul class="nav nav-tabs nav-justified">
  ...
</ul>
<ul class="nav nav-pills nav-justified">
  ...
</ul>

Disabled links

For any nav component (tabs or pills), add .disabled for gray links and no hover effects.
Link functionality not impacted

This class will only change the <a>'s appearance, not its functionality. Use custom JavaScript to disable links here.

    Clickable link
    Clickable link
    Disabled link



<ul class="nav nav-pills">
  ...
  <li role="presentation" class="disabled"><a href="#">Disabled link</a></li>
  ...
</ul>

Using dropdowns

Add dropdown menus with a little extra HTML and the dropdowns JavaScript plugin.
Tabs with dropdowns

    Home
    Help
    Dropdown



<ul class="nav nav-tabs">
  ...
  <li role="presentation" class="dropdown">
    <a class="dropdown-toggle" data-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false">
      Dropdown <span class="caret"></span>
    </a>
    <ul class="dropdown-menu">
      ...
    </ul>
  </li>
  ...
</ul>

Pills with dropdowns

    Home
    Help
    Dropdown



<ul class="nav nav-pills">
  ...
  <li role="presentation" class="dropdown">
    <a class="dropdown-toggle" data-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false">
      Dropdown <span class="caret"></span>
    </a>
    <ul class="dropdown-menu">
      ...
    </ul>
  </li>
  ...
</ul>

Navbar
Default navbar

Navbars are responsive meta components that serve as navigation headers for your application or site. They begin collapsed (and are toggleable) in mobile views and become horizontal as the available viewport width increases.

Justified navbar nav links are currently not supported.
Overflowing content

Since Bootstrap doesn't know how much space the content in your navbar needs, you might run into issues with content wrapping into a second row. To resolve this, you can:

    Reduce the amount or width of navbar items.
    Hide certain navbar items at certain screen sizes using responsive utility classes.
    Change the point at which your navbar switches between collapsed and horizontal mode. Customize the @grid-float-breakpoint variable or add your own media query.

Requires JavaScript plugin

If JavaScript is disabled and the viewport is narrow enough that the navbar collapses, it will be impossible to expand the navbar and view the content within the .navbar-collapse.

The responsive navbar requires the collapse plugin to be included in your version of Bootstrap.
Changing the collapsed mobile navbar breakpoint

The navbar collapses into its vertical mobile view when the viewport is narrower than @grid-float-breakpoint, and expands into its horizontal non-mobile view when the viewport is at least @grid-float-breakpoint in width. Adjust this variable in the Less source to control when the navbar collapses/expands. The default value is 768px (the smallest "small" or "tablet" screen).
Make navbars accessible

Be sure to use a <nav> element or, if using a more generic element such as a <div>, add a role="navigation" to every navbar to explicitly identify it as a landmark region for users of assistive technologies.
Brand

    Link (current)
    Link
    Dropdown

    Link
    Dropdown



<nav class="navbar navbar-default">
  <div class="container-fluid">
    <!-- Brand and toggle get grouped for better mobile display -->
    <div class="navbar-header">
      <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#bs-example-navbar-collapse-1" aria-expanded="false">
        <span class="sr-only">Toggle navigation</span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
      </button>
      <a class="navbar-brand" href="#">Brand</a>
    </div>

    <!-- Collect the nav links, forms, and other content for toggling -->
    <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1">
      <ul class="nav navbar-nav">
        <li class="active"><a href="#">Link <span class="sr-only">(current)</span></a></li>
        <li><a href="#">Link</a></li>
        <li class="dropdown">
          <a href="#" class="dropdown-toggle" data-toggle="dropdown" role="button" aria-haspopup="true" aria-expanded="false">Dropdown <span class="caret"></span></a>
          <ul class="dropdown-menu">
            <li><a href="#">Action</a></li>
            <li><a href="#">Another action</a></li>
            <li><a href="#">Something else here</a></li>
            <li role="separator" class="divider"></li>
            <li><a href="#">Separated link</a></li>
            <li role="separator" class="divider"></li>
            <li><a href="#">One more separated link</a></li>
          </ul>
        </li>
      </ul>
      <form class="navbar-form navbar-left">
        <div class="form-group">
          <input type="text" class="form-control" placeholder="Search">
        </div>
        <button type="submit" class="btn btn-default">Submit</button>
      </form>
      <ul class="nav navbar-nav navbar-right">
        <li><a href="#">Link</a></li>
        <li class="dropdown">
          <a href="#" class="dropdown-toggle" data-toggle="dropdown" role="button" aria-haspopup="true" aria-expanded="false">Dropdown <span class="caret"></span></a>
          <ul class="dropdown-menu">
            <li><a href="#">Action</a></li>
            <li><a href="#">Another action</a></li>
            <li><a href="#">Something else here</a></li>
            <li role="separator" class="divider"></li>
            <li><a href="#">Separated link</a></li>
          </ul>
        </li>
      </ul>
    </div><!-- /.navbar-collapse -->
  </div><!-- /.container-fluid -->
</nav>

Brand image

Replace the navbar brand with your own image by swapping the text for an <img>. Since the .navbar-brand has its own padding and height, you may need to override some CSS depending on your image.
Brand


<nav class="navbar navbar-default">
  <div class="container-fluid">
    <div class="navbar-header">
      <a class="navbar-brand" href="#">
        <img alt="Brand" src="...">
      </a>
    </div>
  </div>
</nav>

Forms

Place form content within .navbar-form for proper vertical alignment and collapsed behavior in narrow viewports. Use the alignment options to decide where it resides within the navbar content.

As a heads up, .navbar-form shares much of its code with .form-inline via mixin. Some form controls, like input groups, may require fixed widths to be show up properly within a navbar.
Brand


<form class="navbar-form navbar-left" role="search">
  <div class="form-group">
    <input type="text" class="form-control" placeholder="Search">
  </div>
  <button type="submit" class="btn btn-default">Submit</button>
</form>

Mobile device caveats

There are some caveats regarding using form controls within fixed elements on mobile devices. See our browser support docs for details.
Always add labels

Screen readers will have trouble with your forms if you don't include a label for every input. For these inline forms, you can hide the labels using the .sr-only class. There are further alternative methods of providing a label for assistive technologies, such as the aria-label, aria-labelledby or title attribute. If none of these is present, screen readers may resort to using the placeholder attribute, if present, but note that use of placeholder as a replacement for other labelling methods is not advised.
Buttons

Add the .navbar-btn class to <button> elements not residing in a <form> to vertically center them in the navbar.
Brand


<button type="button" class="btn btn-default navbar-btn">Sign in</button>

Context-specific usage

Like the standard button classes, .navbar-btn can be used on <a> and <input> elements. However, neither .navbar-btn nor the standard button classes should be used on <a> elements within .navbar-nav.
Text

Wrap strings of text in an element with .navbar-text, usually on a <p> tag for proper leading and color.
Brand

Signed in as Mark Otto


<p class="navbar-text">Signed in as Mark Otto</p>

Non-nav links

For folks using standard links that are not within the regular navbar navigation component, use the .navbar-link class to add the proper colors for the default and inverse navbar options.
Brand

Signed in as Mark Otto


<p class="navbar-text navbar-right">Signed in as <a href="#" class="navbar-link">Mark Otto</a></p>

Component alignment

Align nav links, forms, buttons, or text, using the .navbar-left or .navbar-right utility classes. Both classes will add a CSS float in the specified direction. For example, to align nav links, put them in a separate <ul> with the respective utility class applied.

These classes are mixin-ed versions of .pull-left and .pull-right, but they're scoped to media queries for easier handling of navbar components across device sizes.
Right aligning multiple components

Navbars currently have a limitation with multiple .navbar-right classes. To properly space content, we use negative margin on the last .navbar-right element. When there are multiple elements using that class, these margins don't work as intended.

We'll revisit this when we can rewrite that component in v4.
Fixed to top

Add .navbar-fixed-top and include a .container or .container-fluid to center and pad navbar content.
Brand

    Home
    Link
    Link



<nav class="navbar navbar-default navbar-fixed-top">
  <div class="container">
    ...
  </div>
</nav>

Body padding required

The fixed navbar will overlay your other content, unless you add padding to the top of the <body>. Try out your own values or use our snippet below. Tip: By default, the navbar is 50px high.


body { padding-top: 70px; }

Make sure to include this after the core Bootstrap CSS.
Fixed to bottom

Add .navbar-fixed-bottom and include a .container or .container-fluid to center and pad navbar content.
Brand

    Home
    Link
    Link



<nav class="navbar navbar-default navbar-fixed-bottom">
  <div class="container">
    ...
  </div>
</nav>

Body padding required

The fixed navbar will overlay your other content, unless you add padding to the bottom of the <body>. Try out your own values or use our snippet below. Tip: By default, the navbar is 50px high.


body { padding-bottom: 70px; }

Make sure to include this after the core Bootstrap CSS.
Static top

Create a full-width navbar that scrolls away with the page by adding .navbar-static-top and include a .container or .container-fluid to center and pad navbar content.

Unlike the .navbar-fixed-* classes, you do not need to change any padding on the body.
Brand

    Home
    Link
    Link



<nav class="navbar navbar-default navbar-static-top">
  <div class="container">
    ...
  </div>
</nav>

Inverted navbar

Modify the look of the navbar by adding .navbar-inverse.
Brand

    Home
    Link
    Link



<nav class="navbar navbar-inverse">
  ...
</nav>

Breadcrumbs

Indicate the current page's location within a navigational hierarchy.

Separators are automatically added in CSS through :before and content.

    Home 

    Home Library 

    Home Library Data 



<ol class="breadcrumb">
  <li><a href="#">Home</a></li>
  <li><a href="#">Library</a></li>
  <li class="active">Data</li>
</ol>

Pagination

Provide pagination links for your site or app with the multi-page pagination component, or the simpler pager alternative.
Default pagination

Simple pagination inspired by Rdio, great for apps and search results. The large block is hard to miss, easily scalable, and provides large click areas.

    «
    1
    2
    3
    4
    5
    »



<nav aria-label="Page navigation">
  <ul class="pagination">
    <li>
      <a href="#" aria-label="Previous">
        <span aria-hidden="true">&laquo;</span>
      </a>
    </li>
    <li><a href="#">1</a></li>
    <li><a href="#">2</a></li>
    <li><a href="#">3</a></li>
    <li><a href="#">4</a></li>
    <li><a href="#">5</a></li>
    <li>
      <a href="#" aria-label="Next">
        <span aria-hidden="true">&raquo;</span>
      </a>
    </li>
  </ul>
</nav>

Labelling the pagination component

The pagination component should be wrapped in a <nav> element to identify it as a navigation section to screen readers and other assistive technologies. In addition, as a page is likely to have more than one such navigation section already (such as the primary navigation in the header, or a sidebar navigation), it is advisable to provide a descriptive aria-label for the <nav> which reflects its purpose. For example, if the pagination component is used to navigate between a set of search results, an appropriate label could be aria-label="Search results pages".
Disabled and active states

Links are customizable for different circumstances. Use .disabled for unclickable links and .active to indicate the current page.

    «
    1 (current)
    2
    3
    4
    5
    »



<nav aria-label="...">
  <ul class="pagination">
    <li class="disabled"><a href="#" aria-label="Previous"><span aria-hidden="true">&laquo;</span></a></li>
    <li class="active"><a href="#">1 <span class="sr-only">(current)</span></a></li>
    ...
  </ul>
</nav>

We recommend that you swap out active or disabled anchors for <span>, or omit the anchor in the case of the previous/next arrows, to remove click functionality while retaining intended styles.


<nav aria-label="...">
  <ul class="pagination">
    <li class="disabled">
      <span>
        <span aria-hidden="true">&laquo;</span>
      </span>
    </li>
    <li class="active">
      <span>1 <span class="sr-only">(current)</span></span>
    </li>
    ...
  </ul>
</nav>

Sizing

Fancy larger or smaller pagination? Add .pagination-lg or .pagination-sm for additional sizes.

    «
    1
    2
    3
    4
    5
    »

    «
    1
    2
    3
    4
    5
    »

    «
    1
    2
    3
    4
    5
    »



<nav aria-label="..."><ul class="pagination pagination-lg">...</ul></nav>
<nav aria-label="..."><ul class="pagination">...</ul></nav>
<nav aria-label="..."><ul class="pagination pagination-sm">...</ul></nav>

Pager

Quick previous and next links for simple pagination implementations with light markup and styles. It's great for simple sites like blogs or magazines.
Default example

By default, the pager centers links.

    Previous Next 



<nav aria-label="...">
  <ul class="pager">
    <li><a href="#">Previous</a></li>
    <li><a href="#">Next</a></li>
  </ul>
</nav>

Aligned links

Alternatively, you can align each link to the sides:

    ← Older
    Newer →



<nav aria-label="...">
  <ul class="pager">
    <li class="previous"><a href="#"><span aria-hidden="true">&larr;</span> Older</a></li>
    <li class="next"><a href="#">Newer <span aria-hidden="true">&rarr;</span></a></li>
  </ul>
</nav>

Optional disabled state

Pager links also use the general .disabled utility class from the pagination.

    ← Older
    Newer →



<nav aria-label="...">
  <ul class="pager">
    <li class="previous disabled"><a href="#"><span aria-hidden="true">&larr;</span> Older</a></li>
    <li class="next"><a href="#">Newer <span aria-hidden="true">&rarr;</span></a></li>
  </ul>
</nav>

Labels
Example
Example heading New
Example heading New
Example heading New
Example heading New
Example heading New
Example heading New


<h3>Example heading <span class="label label-default">New</span></h3>

Available variations

Add any of the below mentioned modifier classes to change the appearance of a label.
Default Primary Success Info Warning Danger


<span class="label label-default">Default</span>
<span class="label label-primary">Primary</span>
<span class="label label-success">Success</span>
<span class="label label-info">Info</span>
<span class="label label-warning">Warning</span>
<span class="label label-danger">Danger</span>

Have tons of labels?

Rendering problems can arise when you have dozens of inline labels within a narrow container, each containing its own inline-block element (like an icon). The way around this is setting display: inline-block;. For context and an example, see #13219.
Badges

Easily highlight new or unread items by adding a <span class="badge"> to links, Bootstrap navs, and more.
Inbox 42



<a href="#">Inbox <span class="badge">42</span></a>

<button class="btn btn-primary" type="button">
  Messages <span class="badge">4</span>
</button>

Self collapsing

When there are no new or unread items, badges will simply collapse (via CSS's :empty selector) provided no content exists within.
Cross-browser compatibility

Badges won't self collapse in Internet Explorer 8 because it lacks support for the :empty selector.
Adapts to active nav states

Built-in styles are included for placing badges in active states in pill navigations.

    Home 42
    Profile
    Messages 3



<ul class="nav nav-pills" role="tablist">
  <li role="presentation" class="active"><a href="#">Home <span class="badge">42</span></a></li>
  <li role="presentation"><a href="#">Profile</a></li>
  <li role="presentation"><a href="#">Messages <span class="badge">3</span></a></li>
</ul>

Jumbotron

A lightweight, flexible component that can optionally extend the entire viewport to showcase key content on your site.
Hello, world!

This is a simple hero unit, a simple jumbotron-style component for calling extra attention to featured content or information.



<div class="jumbotron">
  <h1>Hello, world!</h1>
  <p>...</p>
  <p><a class="btn btn-primary btn-lg" href="#" role="button">Learn more</a></p>
</div>

To make the jumbotron full width, and without rounded corners, place it outside all .containers and instead add a .container within.


<div class="jumbotron">
  <div class="container">
    ...
  </div>
</div>

Page header

A simple shell for an h1 to appropriately space out and segment sections of content on a page. It can utilize the h1's default small element, as well as most other components (with additional styles).
Example page header Subtext for header


<div class="page-header">
  <h1>Example page header <small>Subtext for header</small></h1>
</div>

Thumbnails

Extend Bootstrap's grid system with the thumbnail component to easily display grids of images, videos, text, and more.

If you're looking for Pinterest-like presentation of thumbnails of varying heights and/or widths, you'll need to use a third-party plugin such as Masonry, Isotope, or Salvattore.
Default example

By default, Bootstrap's thumbnails are designed to showcase linked images with minimal required markup.
100%x180
100%x180
100%x180
100%x180


<div class="row">
  <div class="col-xs-6 col-md-3">
    <a href="#" class="thumbnail">
      <img src="..." alt="...">
    </a>
  </div>
  ...
</div>

Custom content

With a bit of extra markup, it's possible to add any kind of HTML content like headings, paragraphs, or buttons into thumbnails.
100%x200
Thumbnail label

Cras justo odio, dapibus ac facilisis in, egestas eget quam. Donec id elit non mi porta gravida at eget metus. Nullam id dolor id nibh ultricies vehicula ut id elit.

100%x200
Thumbnail label

Cras justo odio, dapibus ac facilisis in, egestas eget quam. Donec id elit non mi porta gravida at eget metus. Nullam id dolor id nibh ultricies vehicula ut id elit.

100%x200
Thumbnail label

Cras justo odio, dapibus ac facilisis in, egestas eget quam. Donec id elit non mi porta gravida at eget metus. Nullam id dolor id nibh ultricies vehicula ut id elit.



<div class="row">
  <div class="col-sm-6 col-md-4">
    <div class="thumbnail">
      <img src="..." alt="...">
      <div class="caption">
        <h3>Thumbnail label</h3>
        <p>...</p>
        <p><a href="#" class="btn btn-primary" role="button">Button</a> <a href="#" class="btn btn-default" role="button">Button</a></p>
      </div>
    </div>
  </div>
</div>

Alerts

Provide contextual feedback messages for typical user actions with the handful of available and flexible alert messages.
Examples

Wrap any text and an optional dismiss button in .alert and one of the four contextual classes (e.g., .alert-success) for basic alert messages.
No default class

Alerts don't have default classes, only base and modifier classes. A default gray alert doesn't make too much sense, so you're required to specify a type via contextual class. Choose from success, info, warning, or danger.
Well done! You successfully read this important alert message.
Heads up! This alert needs your attention, but it's not super important.
Warning! Better check yourself, you're not looking too good.
Oh snap! Change a few things up and try submitting again.


<div class="alert alert-success" role="alert">...</div>
<div class="alert alert-info" role="alert">...</div>
<div class="alert alert-warning" role="alert">...</div>
<div class="alert alert-danger" role="alert">...</div>

Dismissible alerts

Build on any alert by adding an optional .alert-dismissible and close button.
Requires JavaScript alert plugin

For fully functioning, dismissible alerts, you must use the alerts JavaScript plugin.
Warning! Better check yourself, you're not looking too good.


<div class="alert alert-warning alert-dismissible" role="alert">
  <button type="button" class="close" data-dismiss="alert" aria-label="Close"><span aria-hidden="true">&times;</span></button>
  <strong>Warning!</strong> Better check yourself, you're not looking too good.
</div>

Ensure proper behavior across all devices

Be sure to use the <button> element with the data-dismiss="alert" data attribute.
Links in alerts

Use the .alert-link utility class to quickly provide matching colored links within any alert.
Well done! You successfully read this important alert message.
Heads up! This alert needs your attention, but it's not super important.
Warning! Better check yourself, you're not looking too good.
Oh snap! Change a few things up and try submitting again.


<div class="alert alert-success" role="alert">
  <a href="#" class="alert-link">...</a>
</div>
<div class="alert alert-info" role="alert">
  <a href="#" class="alert-link">...</a>
</div>
<div class="alert alert-warning" role="alert">
  <a href="#" class="alert-link">...</a>
</div>
<div class="alert alert-danger" role="alert">
  <a href="#" class="alert-link">...</a>
</div>

Progress bars

Provide up-to-date feedback on the progress of a workflow or action with simple yet flexible progress bars.
Cross-browser compatibility

Progress bars use CSS3 transitions and animations to achieve some of their effects. These features are not supported in Internet Explorer 9 and below or older versions of Firefox. Opera 12 does not support animations.
Content Security Policy (CSP) compatibility

If your website has a Content Security Policy (CSP) which doesn't allow style-src 'unsafe-inline', then you won't be able to use inline style attributes to set progress bar widths as shown in our examples below. Alternative methods for setting the widths that are compatible with strict CSPs include using a little custom JavaScript (that sets element.style.width) or using custom CSS classes.
Basic example

Default progress bar.
60% Complete


<div class="progress">
  <div class="progress-bar" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" style="width: 60%;">
    <span class="sr-only">60% Complete</span>
  </div>
</div>

With label

Remove the <span> with .sr-only class from within the progress bar to show a visible percentage.
60%


<div class="progress">
  <div class="progress-bar" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" style="width: 60%;">
    60%
  </div>
</div>

To ensure that the label text remains legible even for low percentages, consider adding a min-width to the progress bar.
0%
2%


<div class="progress">
  <div class="progress-bar" role="progressbar" aria-valuenow="0" aria-valuemin="0" aria-valuemax="100" style="min-width: 2em;">
    0%
  </div>
</div>
<div class="progress">
  <div class="progress-bar" role="progressbar" aria-valuenow="2" aria-valuemin="0" aria-valuemax="100" style="min-width: 2em; width: 2%;">
    2%
  </div>
</div>

Contextual alternatives

Progress bars use some of the same button and alert classes for consistent styles.
40% Complete (success)
20% Complete
60% Complete (warning)
80% Complete (danger)


<div class="progress">
  <div class="progress-bar progress-bar-success" role="progressbar" aria-valuenow="40" aria-valuemin="0" aria-valuemax="100" style="width: 40%">
    <span class="sr-only">40% Complete (success)</span>
  </div>
</div>
<div class="progress">
  <div class="progress-bar progress-bar-info" role="progressbar" aria-valuenow="20" aria-valuemin="0" aria-valuemax="100" style="width: 20%">
    <span class="sr-only">20% Complete</span>
  </div>
</div>
<div class="progress">
  <div class="progress-bar progress-bar-warning" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" style="width: 60%">
    <span class="sr-only">60% Complete (warning)</span>
  </div>
</div>
<div class="progress">
  <div class="progress-bar progress-bar-danger" role="progressbar" aria-valuenow="80" aria-valuemin="0" aria-valuemax="100" style="width: 80%">
    <span class="sr-only">80% Complete (danger)</span>
  </div>
</div>

Striped

Uses a gradient to create a striped effect. Not available in IE9 and below.
40% Complete (success)
20% Complete
60% Complete (warning)
80% Complete (danger)


<div class="progress">
  <div class="progress-bar progress-bar-success progress-bar-striped" role="progressbar" aria-valuenow="40" aria-valuemin="0" aria-valuemax="100" style="width: 40%">
    <span class="sr-only">40% Complete (success)</span>
  </div>
</div>
<div class="progress">
  <div class="progress-bar progress-bar-info progress-bar-striped" role="progressbar" aria-valuenow="20" aria-valuemin="0" aria-valuemax="100" style="width: 20%">
    <span class="sr-only">20% Complete</span>
  </div>
</div>
<div class="progress">
  <div class="progress-bar progress-bar-warning progress-bar-striped" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" style="width: 60%">
    <span class="sr-only">60% Complete (warning)</span>
  </div>
</div>
<div class="progress">
  <div class="progress-bar progress-bar-danger progress-bar-striped" role="progressbar" aria-valuenow="80" aria-valuemin="0" aria-valuemax="100" style="width: 80%">
    <span class="sr-only">80% Complete (danger)</span>
  </div>
</div>

Animated

Add .active to .progress-bar-striped to animate the stripes right to left. Not available in IE9 and below.
45% Complete


<div class="progress">
  <div class="progress-bar progress-bar-striped active" role="progressbar" aria-valuenow="45" aria-valuemin="0" aria-valuemax="100" style="width: 45%">
    <span class="sr-only">45% Complete</span>
  </div>
</div>

Stacked

Place multiple bars into the same .progress to stack them.
35% Complete (success)
20% Complete (warning)
10% Complete (danger)


<div class="progress">
  <div class="progress-bar progress-bar-success" style="width: 35%">
    <span class="sr-only">35% Complete (success)</span>
  </div>
  <div class="progress-bar progress-bar-warning progress-bar-striped" style="width: 20%">
    <span class="sr-only">20% Complete (warning)</span>
  </div>
  <div class="progress-bar progress-bar-danger" style="width: 10%">
    <span class="sr-only">10% Complete (danger)</span>
  </div>
</div>

Media object

Abstract object styles for building various types of components (like blog comments, Tweets, etc) that feature a left- or right-aligned image alongside textual content.
Default media

The default media displays a media object (images, video, audio) to the left or right of a content block.
64x64
Media heading
Cras sit amet nibh libero, in gravida nulla. Nulla vel metus scelerisque ante sollicitudin commodo. Cras purus odio, vestibulum in vulputate at, tempus viverra turpis. Fusce condimentum nunc ac nisi vulputate fringilla. Donec lacinia congue felis in faucibus.
64x64
Media heading
Cras sit amet nibh libero, in gravida nulla. Nulla vel metus scelerisque ante sollicitudin commodo. Cras purus odio, vestibulum in vulputate at, tempus viverra turpis. Fusce condimentum nunc ac nisi vulputate fringilla. Donec lacinia congue felis in faucibus.
64x64
Nested media heading
Cras sit amet nibh libero, in gravida nulla. Nulla vel metus scelerisque ante sollicitudin commodo. Cras purus odio, vestibulum in vulputate at, tempus viverra turpis. Fusce condimentum nunc ac nisi vulputate fringilla. Donec lacinia congue felis in faucibus.
Media heading
Cras sit amet nibh libero, in gravida nulla. Nulla vel metus scelerisque ante sollicitudin commodo. Cras purus odio, vestibulum in vulputate at, tempus viverra turpis.
64x64
64x64
Media heading
Cras sit amet nibh libero, in gravida nulla. Nulla vel metus scelerisque ante sollicitudin commodo. Cras purus odio, vestibulum in vulputate at, tempus viverra turpis.
64x64


<div class="media">
  <div class="media-left">
    <a href="#">
      <img class="media-object" src="..." alt="...">
    </a>
  </div>
  <div class="media-body">
    <h4 class="media-heading">Media heading</h4>
    ...
  </div>
</div>

The classes .pull-left and .pull-right also exist and were previously used as part of the media component, but are deprecated for that use as of v3.3.0. They are approximately equivalent to .media-left and .media-right, except that .media-right should be placed after the .media-body in the html.
Media alignment

The images or other media can be aligned top, middle, or bottom. The default is top aligned.
64x64
Top aligned media

Cras sit amet nibh libero, in gravida nulla. Nulla vel metus scelerisque ante sollicitudin commodo. Cras purus odio, vestibulum in vulputate at, tempus viverra turpis. Fusce condimentum nunc ac nisi vulputate fringilla. Donec lacinia congue felis in faucibus.

Donec sed odio dui. Nullam quis risus eget urna mollis ornare vel eu leo. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.
64x64
Middle aligned media

Cras sit amet nibh libero, in gravida nulla. Nulla vel metus scelerisque ante sollicitudin commodo. Cras purus odio, vestibulum in vulputate at, tempus viverra turpis. Fusce condimentum nunc ac nisi vulputate fringilla. Donec lacinia congue felis in faucibus.

Donec sed odio dui. Nullam quis risus eget urna mollis ornare vel eu leo. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.
64x64
Bottom aligned media

Cras sit amet nibh libero, in gravida nulla. Nulla vel metus scelerisque ante sollicitudin commodo. Cras purus odio, vestibulum in vulputate at, tempus viverra turpis. Fusce condimentum nunc ac nisi vulputate fringilla. Donec lacinia congue felis in faucibus.

Donec sed odio dui. Nullam quis risus eget urna mollis ornare vel eu leo. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.


<div class="media">
  <div class="media-left media-middle">
    <a href="#">
      <img class="media-object" src="..." alt="...">
    </a>
  </div>
  <div class="media-body">
    <h4 class="media-heading">Middle aligned media</h4>
    ...
  </div>
</div>

Media list

With a bit of extra markup, you can use media inside list (useful for comment threads or articles lists).

    64x64
    Media heading

    Cras sit amet nibh libero, in gravida nulla. Nulla vel metus scelerisque ante sollicitudin commodo. Cras purus odio, vestibulum in vulputate at, tempus viverra turpis.
    64x64
    Nested media heading
    Cras sit amet nibh libero, in gravida nulla. Nulla vel metus scelerisque ante sollicitudin commodo. Cras purus odio, vestibulum in vulputate at, tempus viverra turpis.
    64x64
    Nested media heading
    Cras sit amet nibh libero, in gravida nulla. Nulla vel metus scelerisque ante sollicitudin commodo. Cras purus odio, vestibulum in vulputate at, tempus viverra turpis.
    64x64
    Nested media heading
    Cras sit amet nibh libero, in gravida nulla. Nulla vel metus scelerisque ante sollicitudin commodo. Cras purus odio, vestibulum in vulputate at, tempus viverra turpis.



<ul class="media-list">
  <li class="media">
    <div class="media-left">
      <a href="#">
        <img class="media-object" src="..." alt="...">
      </a>
    </div>
    <div class="media-body">
      <h4 class="media-heading">Media heading</h4>
      ...
    </div>
  </li>
</ul>

List group

List groups are a flexible and powerful component for displaying not only simple lists of elements, but complex ones with custom content.
Basic example

The most basic list group is simply an unordered list with list items, and the proper classes. Build upon it with the options that follow, or your own CSS as needed.

    Cras justo odio
    Dapibus ac facilisis in
    Morbi leo risus
    Porta ac consectetur ac
    Vestibulum at eros



<ul class="list-group">
  <li class="list-group-item">Cras justo odio</li>
  <li class="list-group-item">Dapibus ac facilisis in</li>
  <li class="list-group-item">Morbi leo risus</li>
  <li class="list-group-item">Porta ac consectetur ac</li>
  <li class="list-group-item">Vestibulum at eros</li>
</ul>

Badges

Add the badges component to any list group item and it will automatically be positioned on the right.

    14 Cras justo odio
    2 Dapibus ac facilisis in
    1 Morbi leo risus



<ul class="list-group">
  <li class="list-group-item">
    <span class="badge">14</span>
    Cras justo odio
  </li>
</ul>

Linked items

Linkify list group items by using anchor tags instead of list items (that also means a parent <div> instead of an <ul>). No need for individual parents around each element.
Cras justo odio
Dapibus ac facilisis in
Morbi leo risus
Porta ac consectetur ac
Vestibulum at eros


<div class="list-group">
  <a href="#" class="list-group-item active">
    Cras justo odio
  </a>
  <a href="#" class="list-group-item">Dapibus ac facilisis in</a>
  <a href="#" class="list-group-item">Morbi leo risus</a>
  <a href="#" class="list-group-item">Porta ac consectetur ac</a>
  <a href="#" class="list-group-item">Vestibulum at eros</a>
</div>

Button items

List group items may be buttons instead of list items (that also means a parent <div> instead of an <ul>). No need for individual parents around each element. Don't use the standard .btn classes here.


<div class="list-group">
  <button type="button" class="list-group-item">Cras justo odio</button>
  <button type="button" class="list-group-item">Dapibus ac facilisis in</button>
  <button type="button" class="list-group-item">Morbi leo risus</button>
  <button type="button" class="list-group-item">Porta ac consectetur ac</button>
  <button type="button" class="list-group-item">Vestibulum at eros</button>
</div>

Disabled items

Add .disabled to a .list-group-item to gray it out to appear disabled.
Cras justo odio
Dapibus ac facilisis in
Morbi leo risus
Porta ac consectetur ac
Vestibulum at eros


<div class="list-group">
  <a href="#" class="list-group-item disabled">
    Cras justo odio
  </a>
  <a href="#" class="list-group-item">Dapibus ac facilisis in</a>
  <a href="#" class="list-group-item">Morbi leo risus</a>
  <a href="#" class="list-group-item">Porta ac consectetur ac</a>
  <a href="#" class="list-group-item">Vestibulum at eros</a>
</div>

Contextual classes

Use contextual classes to style list items, default or linked. Also includes .active state.

    Dapibus ac facilisis in
    Cras sit amet nibh libero
    Porta ac consectetur ac
    Vestibulum at eros

Dapibus ac facilisis in
Cras sit amet nibh libero
Porta ac consectetur ac
Vestibulum at eros


<ul class="list-group">
  <li class="list-group-item list-group-item-success">Dapibus ac facilisis in</li>
  <li class="list-group-item list-group-item-info">Cras sit amet nibh libero</li>
  <li class="list-group-item list-group-item-warning">Porta ac consectetur ac</li>
  <li class="list-group-item list-group-item-danger">Vestibulum at eros</li>
</ul>
<div class="list-group">
  <a href="#" class="list-group-item list-group-item-success">Dapibus ac facilisis in</a>
  <a href="#" class="list-group-item list-group-item-info">Cras sit amet nibh libero</a>
  <a href="#" class="list-group-item list-group-item-warning">Porta ac consectetur ac</a>
  <a href="#" class="list-group-item list-group-item-danger">Vestibulum at eros</a>
</div>

Custom content

Add nearly any HTML within, even for linked list groups like the one below.
List group item heading

Donec id elit non mi porta gravida at eget metus. Maecenas sed diam eget risus varius blandit.
List group item heading

Donec id elit non mi porta gravida at eget metus. Maecenas sed diam eget risus varius blandit.
List group item heading

Donec id elit non mi porta gravida at eget metus. Maecenas sed diam eget risus varius blandit.


<div class="list-group">
  <a href="#" class="list-group-item active">
    <h4 class="list-group-item-heading">List group item heading</h4>
    <p class="list-group-item-text">...</p>
  </a>
</div>

Panels

While not always necessary, sometimes you need to put your DOM in a box. For those situations, try the panel component.
Basic example

By default, all the .panel does is apply some basic border and padding to contain some content.
Basic panel example


<div class="panel panel-default">
  <div class="panel-body">
    Basic panel example
  </div>
</div>

Panel with heading

Easily add a heading container to your panel with .panel-heading. You may also include any <h1>-<h6> with a .panel-title class to add a pre-styled heading. However, the font sizes of <h1>-<h6> are overridden by .panel-heading.

For proper link coloring, be sure to place links in headings within .panel-title.
Panel heading without title
Panel content
Panel title
Panel content


<div class="panel panel-default">
  <div class="panel-heading">Panel heading without title</div>
  <div class="panel-body">
    Panel content
  </div>
</div>

<div class="panel panel-default">
  <div class="panel-heading">
    <h3 class="panel-title">Panel title</h3>
  </div>
  <div class="panel-body">
    Panel content
  </div>
</div>

Panel with footer

Wrap buttons or secondary text in .panel-footer. Note that panel footers do not inherit colors and borders when using contextual variations as they are not meant to be in the foreground.
Panel content
Panel footer


<div class="panel panel-default">
  <div class="panel-body">
    Panel content
  </div>
  <div class="panel-footer">Panel footer</div>
</div>

Contextual alternatives

Like other components, easily make a panel more meaningful to a particular context by adding any of the contextual state classes.
Panel title
Panel content
Panel title
Panel content
Panel title
Panel content
Panel title
Panel content
Panel title
Panel content


<div class="panel panel-primary">...</div>
<div class="panel panel-success">...</div>
<div class="panel panel-info">...</div>
<div class="panel panel-warning">...</div>
<div class="panel panel-danger">...</div>

With tables

Add any non-bordered .table within a panel for a seamless design. If there is a .panel-body, we add an extra border to the top of the table for separation.
Panel heading

Some default panel content here. Nulla vitae elit libero, a pharetra augue. Aenean lacinia bibendum nulla sed consectetur. Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum. Nullam id dolor id nibh ultricies vehicula ut id elit.
# 	First Name 	Last Name 	Username
1 	Mark 	Otto 	@mdo
2 	Jacob 	Thornton 	@fat
3 	Larry 	the Bird 	@twitter


<div class="panel panel-default">
  <!-- Default panel contents -->
  <div class="panel-heading">Panel heading</div>
  <div class="panel-body">
    <p>...</p>
  </div>

  <!-- Table -->
  <table class="table">
    ...
  </table>
</div>

If there is no panel body, the component moves from panel header to table without interruption.
Panel heading
# 	First Name 	Last Name 	Username
1 	Mark 	Otto 	@mdo
2 	Jacob 	Thornton 	@fat
3 	Larry 	the Bird 	@twitter


<div class="panel panel-default">
  <!-- Default panel contents -->
  <div class="panel-heading">Panel heading</div>

  <!-- Table -->
  <table class="table">
    ...
  </table>
</div>

With list groups

Easily include full-width list groups within any panel.
Panel heading

Some default panel content here. Nulla vitae elit libero, a pharetra augue. Aenean lacinia bibendum nulla sed consectetur. Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum. Nullam id dolor id nibh ultricies vehicula ut id elit.

    Cras justo odio
    Dapibus ac facilisis in
    Morbi leo risus
    Porta ac consectetur ac
    Vestibulum at eros



<div class="panel panel-default">
  <!-- Default panel contents -->
  <div class="panel-heading">Panel heading</div>
  <div class="panel-body">
    <p>...</p>
  </div>

  <!-- List group -->
  <ul class="list-group">
    <li class="list-group-item">Cras justo odio</li>
    <li class="list-group-item">Dapibus ac facilisis in</li>
    <li class="list-group-item">Morbi leo risus</li>
    <li class="list-group-item">Porta ac consectetur ac</li>
    <li class="list-group-item">Vestibulum at eros</li>
  </ul>
</div>

Responsive embed

Allow browsers to determine video or slideshow dimensions based on the width of their containing block by creating an intrinsic ratio that will properly scale on any device.

Rules are directly applied to <iframe>, <embed>, <video>, and <object> elements; optionally use an explicit descendant class .embed-responsive-item when you want to match the styling for other attributes.

Pro-Tip! You don't need to include frameborder="0" in your <iframe>s as we override that for you.


<!-- 16:9 aspect ratio -->
<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="..."></iframe>
</div>

<!-- 4:3 aspect ratio -->
<div class="embed-responsive embed-responsive-4by3">
  <iframe class="embed-responsive-item" src="..."></iframe>
</div>

Wells
Default well

Use the well as a simple effect on an element to give it an inset effect.
Look, I'm in a well!


<div class="well">...</div>

Optional classes

Control padding and rounded corners with two optional modifier classes.
Look, I'm in a large well!


<div class="well well-lg">...</div>

Look, I'm in a small well!


<div class="well well-sm">...</div>
-------------------------------------------------------------------------------

JavaScript

Bring Bootstrap's components to life with over a dozen custom jQuery plugins. Easily include them all, or one by one.
Overview
Individual or compiled

Plugins can be included individually (using Bootstrap's individual *.js files), or all at once (using bootstrap.js or the minified bootstrap.min.js).
Using the compiled JavaScript

Both bootstrap.js and bootstrap.min.js contain all plugins in a single file. Include only one.
Plugin dependencies

Some plugins and CSS components depend on other plugins. If you include plugins individually, make sure to check for these dependencies in the docs. Also note that all plugins depend on jQuery (this means jQuery must be included before the plugin files). Consult our bower.json to see which versions of jQuery are supported.
Data attributes

You can use all Bootstrap plugins purely through the markup API without writing a single line of JavaScript. This is Bootstrap's first-class API and should be your first consideration when using a plugin.

That said, in some situations it may be desirable to turn this functionality off. Therefore, we also provide the ability to disable the data attribute API by unbinding all events on the document namespaced with data-api. This looks like this:


$(document).off('.data-api')

Alternatively, to target a specific plugin, just include the plugin's name as a namespace along with the data-api namespace like this:


$(document).off('.alert.data-api')

Only one plugin per element via data attributes

Don't use data attributes from multiple plugins on the same element. For example, a button cannot both have a tooltip and toggle a modal. To accomplish this, use a wrapping element.
Programmatic API

We also believe you should be able to use all Bootstrap plugins purely through the JavaScript API. All public APIs are single, chainable methods, and return the collection acted upon.


$('.btn.danger').button('toggle').addClass('fat')

All methods should accept an optional options object, a string which targets a particular method, or nothing (which initiates a plugin with default behavior):


$('#myModal').modal()                      // initialized with defaults
$('#myModal').modal({ keyboard: false })   // initialized with no keyboard
$('#myModal').modal('show')                // initializes and invokes show immediately

Each plugin also exposes its raw constructor on a Constructor property: $.fn.popover.Constructor. If you'd like to get a particular plugin instance, retrieve it directly from an element: $('[rel="popover"]').data('popover').
Default settings

You can change the default settings for a plugin by modifying the plugin's Constructor.DEFAULTS object:


$.fn.modal.Constructor.DEFAULTS.keyboard = false // changes default for the modal plugin's `keyboard` option to false

No conflict

Sometimes it is necessary to use Bootstrap plugins with other UI frameworks. In these circumstances, namespace collisions can occasionally occur. If this happens, you may call .noConflict on the plugin you wish to revert the value of.


var bootstrapButton = $.fn.button.noConflict() // return $.fn.button to previously assigned value
$.fn.bootstrapBtn = bootstrapButton            // give $().bootstrapBtn the Bootstrap functionality

Events

Bootstrap provides custom events for most plugins' unique actions. Generally, these come in an infinitive and past participle form - where the infinitive (ex. show) is triggered at the start of an event, and its past participle form (ex. shown) is triggered on the completion of an action.

As of 3.0.0, all Bootstrap events are namespaced.

All infinitive events provide preventDefault functionality. This provides the ability to stop the execution of an action before it starts.


$('#myModal').on('show.bs.modal', function (e) {
  if (!data) return e.preventDefault() // stops modal from being shown
})

Version numbers

The version of each of Bootstrap's jQuery plugins can be accessed via the VERSION property of the plugin's constructor. For example, for the tooltip plugin:


$.fn.tooltip.Constructor.VERSION // => "3.3.7"

No special fallbacks when JavaScript is disabled

Bootstrap's plugins don't fall back particularly gracefully when JavaScript is disabled. If you care about the user experience in this case, use <noscript> to explain the situation (and how to re-enable JavaScript) to your users, and/or add your own custom fallbacks.
Third-party libraries

Bootstrap does not officially support third-party JavaScript libraries like Prototype or jQuery UI. Despite .noConflict and namespaced events, there may be compatibility problems that you need to fix on your own.
Transitions transition.js
About transitions

For simple transition effects, include transition.js once alongside the other JS files. If you're using the compiled (or minified) bootstrap.js, there is no need to include this—it's already there.
What's inside

Transition.js is a basic helper for transitionEnd events as well as a CSS transition emulator. It's used by the other plugins to check for CSS transition support and to catch hanging transitions.
Disabling transitions

Transitions can be globally disabled using the following JavaScript snippet, which must come after transition.js (or bootstrap.js or bootstrap.min.js, as the case may be) has loaded:


$.support.transition = false

Modals modal.js

Modals are streamlined, but flexible, dialog prompts with the minimum required functionality and smart defaults.
Multiple open modals not supported

Be sure not to open a modal while another is still visible. Showing more than one modal at a time requires custom code.
Modal markup placement

Always try to place a modal's HTML code in a top-level position in your document to avoid other components affecting the modal's appearance and/or functionality.
Mobile device caveats

There are some caveats regarding using modals on mobile devices. See our browser support docs for details.

Due to how HTML5 defines its semantics, the autofocus HTML attribute has no effect in Bootstrap modals. To achieve the same effect, use some custom JavaScript:


$('#myModal').on('shown.bs.modal', function () {
  $('#myInput').focus()
})

Examples
Static example

A rendered modal with header, body, and set of actions in the footer.
Modal title

One fine body…


<div class="modal fade" tabindex="-1" role="dialog">
  <div class="modal-dialog" role="document">
    <div class="modal-content">
      <div class="modal-header">
        <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
        <h4 class="modal-title">Modal title</h4>
      </div>
      <div class="modal-body">
        <p>One fine body&hellip;</p>
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-default" data-dismiss="modal">Close</button>
        <button type="button" class="btn btn-primary">Save changes</button>
      </div>
    </div><!-- /.modal-content -->
  </div><!-- /.modal-dialog -->
</div><!-- /.modal -->

Live demo

Toggle a modal via JavaScript by clicking the button below. It will slide down and fade in from the top of the page.


<!-- Button trigger modal -->
<button type="button" class="btn btn-primary btn-lg" data-toggle="modal" data-target="#myModal">
  Launch demo modal
</button>

<!-- Modal -->
<div class="modal fade" id="myModal" tabindex="-1" role="dialog" aria-labelledby="myModalLabel">
  <div class="modal-dialog" role="document">
    <div class="modal-content">
      <div class="modal-header">
        <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
        <h4 class="modal-title" id="myModalLabel">Modal title</h4>
      </div>
      <div class="modal-body">
        ...
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-default" data-dismiss="modal">Close</button>
        <button type="button" class="btn btn-primary">Save changes</button>
      </div>
    </div>
  </div>
</div>

Make modals accessible

Be sure to add role="dialog" and aria-labelledby="...", referencing the modal title, to .modal, and role="document" to the .modal-dialog itself.

Additionally, you may give a description of your modal dialog with aria-describedby on .modal.
Embedding YouTube videos

Embedding YouTube videos in modals requires additional JavaScript not in Bootstrap to automatically stop playback and more. See this helpful Stack Overflow post for more information.
Optional sizes

Modals have two optional sizes, available via modifier classes to be placed on a .modal-dialog.


<!-- Large modal -->
<button type="button" class="btn btn-primary" data-toggle="modal" data-target=".bs-example-modal-lg">Large modal</button>

<div class="modal fade bs-example-modal-lg" tabindex="-1" role="dialog" aria-labelledby="myLargeModalLabel">
  <div class="modal-dialog modal-lg" role="document">
    <div class="modal-content">
      ...
    </div>
  </div>
</div>

<!-- Small modal -->
<button type="button" class="btn btn-primary" data-toggle="modal" data-target=".bs-example-modal-sm">Small modal</button>

<div class="modal fade bs-example-modal-sm" tabindex="-1" role="dialog" aria-labelledby="mySmallModalLabel">
  <div class="modal-dialog modal-sm" role="document">
    <div class="modal-content">
      ...
    </div>
  </div>
</div>

Remove animation

For modals that simply appear rather than fade in to view, remove the .fade class from your modal markup.


<div class="modal" tabindex="-1" role="dialog" aria-labelledby="...">
  ...
</div>

Using the grid system

To take advantage of the Bootstrap grid system within a modal, just nest .rows within the .modal-body and then use the normal grid system classes.


<div class="modal fade" tabindex="-1" role="dialog" aria-labelledby="gridSystemModalLabel">
  <div class="modal-dialog" role="document">
    <div class="modal-content">
      <div class="modal-header">
        <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
        <h4 class="modal-title" id="gridSystemModalLabel">Modal title</h4>
      </div>
      <div class="modal-body">
        <div class="row">
          <div class="col-md-4">.col-md-4</div>
          <div class="col-md-4 col-md-offset-4">.col-md-4 .col-md-offset-4</div>
        </div>
        <div class="row">
          <div class="col-md-3 col-md-offset-3">.col-md-3 .col-md-offset-3</div>
          <div class="col-md-2 col-md-offset-4">.col-md-2 .col-md-offset-4</div>
        </div>
        <div class="row">
          <div class="col-md-6 col-md-offset-3">.col-md-6 .col-md-offset-3</div>
        </div>
        <div class="row">
          <div class="col-sm-9">
            Level 1: .col-sm-9
            <div class="row">
              <div class="col-xs-8 col-sm-6">
                Level 2: .col-xs-8 .col-sm-6
              </div>
              <div class="col-xs-4 col-sm-6">
                Level 2: .col-xs-4 .col-sm-6
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-default" data-dismiss="modal">Close</button>
        <button type="button" class="btn btn-primary">Save changes</button>
      </div>
    </div><!-- /.modal-content -->
  </div><!-- /.modal-dialog -->
</div><!-- /.modal -->

Varying modal content based on trigger button

Have a bunch of buttons that all trigger the same modal, just with slightly different contents? Use event.relatedTarget and HTML data-* attributes (possibly via jQuery) to vary the contents of the modal depending on which button was clicked. See the Modal Events docs for details on relatedTarget,
...more buttons...


<button type="button" class="btn btn-primary" data-toggle="modal" data-target="#exampleModal" data-whatever="@mdo">Open modal for @mdo</button>
<button type="button" class="btn btn-primary" data-toggle="modal" data-target="#exampleModal" data-whatever="@fat">Open modal for @fat</button>
<button type="button" class="btn btn-primary" data-toggle="modal" data-target="#exampleModal" data-whatever="@getbootstrap">Open modal for @getbootstrap</button>
...more buttons...

<div class="modal fade" id="exampleModal" tabindex="-1" role="dialog" aria-labelledby="exampleModalLabel">
  <div class="modal-dialog" role="document">
    <div class="modal-content">
      <div class="modal-header">
        <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
        <h4 class="modal-title" id="exampleModalLabel">New message</h4>
      </div>
      <div class="modal-body">
        <form>
          <div class="form-group">
            <label for="recipient-name" class="control-label">Recipient:</label>
            <input type="text" class="form-control" id="recipient-name">
          </div>
          <div class="form-group">
            <label for="message-text" class="control-label">Message:</label>
            <textarea class="form-control" id="message-text"></textarea>
          </div>
        </form>
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-default" data-dismiss="modal">Close</button>
        <button type="button" class="btn btn-primary">Send message</button>
      </div>
    </div>
  </div>
</div>



$('#exampleModal').on('show.bs.modal', function (event) {
  var button = $(event.relatedTarget) // Button that triggered the modal
  var recipient = button.data('whatever') // Extract info from data-* attributes
  // If necessary, you could initiate an AJAX request here (and then do the updating in a callback).
  // Update the modal's content. We'll use jQuery here, but you could use a data binding library or other methods instead.
  var modal = $(this)
  modal.find('.modal-title').text('New message to ' + recipient)
  modal.find('.modal-body input').val(recipient)
})

Usage

The modal plugin toggles your hidden content on demand, via data attributes or JavaScript. It also adds .modal-open to the <body> to override default scrolling behavior and generates a .modal-backdrop to provide a click area for dismissing shown modals when clicking outside the modal.
Via data attributes

Activate a modal without writing JavaScript. Set data-toggle="modal" on a controller element, like a button, along with a data-target="#foo" or href="#foo" to target a specific modal to toggle.


<button type="button" data-toggle="modal" data-target="#myModal">Launch modal</button>

Via JavaScript

Call a modal with id myModal with a single line of JavaScript:


$('#myModal').modal(options)

Options

Options can be passed via data attributes or JavaScript. For data attributes, append the option name to data-, as in data-backdrop="".
Name 	type 	default 	description
backdrop 	boolean or the string 'static' 	true 	Includes a modal-backdrop element. Alternatively, specify static for a backdrop which doesn't close the modal on click.
keyboard 	boolean 	true 	Closes the modal when escape key is pressed
show 	boolean 	true 	Shows the modal when initialized.
remote 	path 	false 	

This option is deprecated since v3.3.0 and has been removed in v4. We recommend instead using client-side templating or a data binding framework, or calling jQuery.load yourself.

If a remote URL is provided, content will be loaded one time via jQuery's load method and injected into the .modal-content div. If you're using the data-api, you may alternatively use the href attribute to specify the remote source. An example of this is shown below:


<a data-toggle="modal" href="remote.html" data-target="#modal">Click me</a>

Methods
.modal(options)

Activates your content as a modal. Accepts an optional options object.


$('#myModal').modal({
  keyboard: false
})

.modal('toggle')

Manually toggles a modal. Returns to the caller before the modal has actually been shown or hidden (i.e. before the shown.bs.modal or hidden.bs.modal event occurs).


$('#myModal').modal('toggle')

.modal('show')

Manually opens a modal. Returns to the caller before the modal has actually been shown (i.e. before the shown.bs.modal event occurs).


$('#myModal').modal('show')

.modal('hide')

Manually hides a modal. Returns to the caller before the modal has actually been hidden (i.e. before the hidden.bs.modal event occurs).


$('#myModal').modal('hide')

.modal('handleUpdate')

Readjusts the modal's positioning to counter a scrollbar in case one should appear, which would make the modal jump to the left.

Only needed when the height of the modal changes while it is open.


$('#myModal').modal('handleUpdate')

Events

Bootstrap's modal class exposes a few events for hooking into modal functionality.

All modal events are fired at the modal itself (i.e. at the <div class="modal">).
Event Type 	Description
show.bs.modal 	This event fires immediately when the show instance method is called. If caused by a click, the clicked element is available as the relatedTarget property of the event.
shown.bs.modal 	This event is fired when the modal has been made visible to the user (will wait for CSS transitions to complete). If caused by a click, the clicked element is available as the relatedTarget property of the event.
hide.bs.modal 	This event is fired immediately when the hide instance method has been called.
hidden.bs.modal 	This event is fired when the modal has finished being hidden from the user (will wait for CSS transitions to complete).
loaded.bs.modal 	This event is fired when the modal has loaded content using the remote option.


$('#myModal').on('hidden.bs.modal', function (e) {
  // do something...
})

Dropdowns dropdown.js
Examples

Add dropdown menus to nearly anything with this simple plugin, including the navbar, tabs, and pills.
Within a navbar
Project Name

    Dropdown
    Dropdown

    Dropdown

Within pills

    Regular link
    Dropdown
    Dropdown
    Dropdown

Usage

Via data attributes or JavaScript, the dropdown plugin toggles hidden content (dropdown menus) by toggling the .open class on the parent list item.

On mobile devices, opening a dropdown adds a .dropdown-backdrop as a tap area for closing dropdown menus when tapping outside the menu, a requirement for proper iOS support. This means that switching from an open dropdown menu to a different dropdown menu requires an extra tap on mobile.

Note: The data-toggle="dropdown" attribute is relied on for closing dropdown menus at an application level, so it's a good idea to always use it.
Via data attributes

Add data-toggle="dropdown" to a link or button to toggle a dropdown.


<div class="dropdown">
  <button id="dLabel" type="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
    Dropdown trigger
    <span class="caret"></span>
  </button>
  <ul class="dropdown-menu" aria-labelledby="dLabel">
    ...
  </ul>
</div>

To keep URLs intact with link buttons, use the data-target attribute instead of href="#".


<div class="dropdown">
  <a id="dLabel" data-target="#" href="http://example.com" data-toggle="dropdown" role="button" aria-haspopup="true" aria-expanded="false">
    Dropdown trigger
    <span class="caret"></span>
  </a>

  <ul class="dropdown-menu" aria-labelledby="dLabel">
    ...
  </ul>
</div>

Via JavaScript

Call the dropdowns via JavaScript:


$('.dropdown-toggle').dropdown()

data-toggle="dropdown" still required

Regardless of whether you call your dropdown via JavaScript or instead use the data-api, data-toggle="dropdown" is always required to be present on the dropdown's trigger element.
Options

None
Methods
$().dropdown('toggle')

Toggles the dropdown menu of a given navbar or tabbed navigation.
Events

All dropdown events are fired at the .dropdown-menu's parent element.

All dropdown events have a relatedTarget property, whose value is the toggling anchor element.
Event Type 	Description
show.bs.dropdown 	This event fires immediately when the show instance method is called.
shown.bs.dropdown 	This event is fired when the dropdown has been made visible to the user (will wait for CSS transitions, to complete).
hide.bs.dropdown 	This event is fired immediately when the hide instance method has been called.
hidden.bs.dropdown 	This event is fired when the dropdown has finished being hidden from the user (will wait for CSS transitions, to complete).


$('#myDropdown').on('show.bs.dropdown', function () {
  // do something…
})

ScrollSpy scrollspy.js
Example in navbar

The ScrollSpy plugin is for automatically updating nav targets based on scroll position. Scroll the area below the navbar and watch the active class change. The dropdown sub items will be highlighted as well.
Project Name

    @fat
    @mdo
    Dropdown

@fat

Ad leggings keytar, brunch id art party dolor labore. Pitchfork yr enim lo-fi before they sold out qui. Tumblr farm-to-table bicycle rights whatever. Anim keffiyeh carles cardigan. Velit seitan mcsweeney's photo booth 3 wolf moon irure. Cosby sweater lomo jean shorts, williamsburg hoodie minim qui you probably haven't heard of them et cardigan trust fund culpa biodiesel wes anderson aesthetic. Nihil tattooed accusamus, cred irony biodiesel keffiyeh artisan ullamco consequat.
@mdo

Veniam marfa mustache skateboard, adipisicing fugiat velit pitchfork beard. Freegan beard aliqua cupidatat mcsweeney's vero. Cupidatat four loko nisi, ea helvetica nulla carles. Tattooed cosby sweater food truck, mcsweeney's quis non freegan vinyl. Lo-fi wes anderson +1 sartorial. Carles non aesthetic exercitation quis gentrify. Brooklyn adipisicing craft beer vice keytar deserunt.
one

Occaecat commodo aliqua delectus. Fap craft beer deserunt skateboard ea. Lomo bicycle rights adipisicing banh mi, velit ea sunt next level locavore single-origin coffee in magna veniam. High life id vinyl, echo park consequat quis aliquip banh mi pitchfork. Vero VHS est adipisicing. Consectetur nisi DIY minim messenger bag. Cred ex in, sustainable delectus consectetur fanny pack iphone.
two

In incididunt echo park, officia deserunt mcsweeney's proident master cleanse thundercats sapiente veniam. Excepteur VHS elit, proident shoreditch +1 biodiesel laborum craft beer. Single-origin coffee wayfarers irure four loko, cupidatat terry richardson master cleanse. Assumenda you probably haven't heard of them art party fanny pack, tattooed nulla cardigan tempor ad. Proident wolf nesciunt sartorial keffiyeh eu banh mi sustainable. Elit wolf voluptate, lo-fi ea portland before they sold out four loko. Locavore enim nostrud mlkshk brooklyn nesciunt.
three

Ad leggings keytar, brunch id art party dolor labore. Pitchfork yr enim lo-fi before they sold out qui. Tumblr farm-to-table bicycle rights whatever. Anim keffiyeh carles cardigan. Velit seitan mcsweeney's photo booth 3 wolf moon irure. Cosby sweater lomo jean shorts, williamsburg hoodie minim qui you probably haven't heard of them et cardigan trust fund culpa biodiesel wes anderson aesthetic. Nihil tattooed accusamus, cred irony biodiesel keffiyeh artisan ullamco consequat.

Keytar twee blog, culpa messenger bag marfa whatever delectus food truck. Sapiente synth id assumenda. Locavore sed helvetica cliche irony, thundercats you probably haven't heard of them consequat hoodie gluten-free lo-fi fap aliquip. Labore elit placeat before they sold out, terry richardson proident brunch nesciunt quis cosby sweater pariatur keffiyeh ut helvetica artisan. Cardigan craft beer seitan readymade velit. VHS chambray laboris tempor veniam. Anim mollit minim commodo ullamco thundercats.
Usage
Requires Bootstrap nav

Scrollspy currently requires the use of a Bootstrap nav component for proper highlighting of active links.
Resolvable ID targets required

Navbar links must have resolvable id targets. For example, a <a href="#home">home</a> must correspond to something in the DOM like <div id="home"></div>.
Non-:visible target elements ignored

Target elements that are not :visible according to jQuery will be ignored and their corresponding nav items will never be highlighted.
Requires relative positioning

No matter the implementation method, scrollspy requires the use of position: relative; on the element you're spying on. In most cases this is the <body>. When scrollspying on elements other than the <body>, be sure to have a height set and overflow-y: scroll; applied.
Via data attributes

To easily add scrollspy behavior to your topbar navigation, add data-spy="scroll" to the element you want to spy on (most typically this would be the <body>). Then add the data-target attribute with the ID or class of the parent element of any Bootstrap .nav component.


body {
  position: relative;
}



<body data-spy="scroll" data-target="#navbar-example">
  ...
  <div id="navbar-example">
    <ul class="nav nav-tabs" role="tablist">
      ...
    </ul>
  </div>
  ...
</body>

Via JavaScript

After adding position: relative; in your CSS, call the scrollspy via JavaScript:


$('body').scrollspy({ target: '#navbar-example' })

Methods
.scrollspy('refresh')

When using scrollspy in conjunction with adding or removing of elements from the DOM, you'll need to call the refresh method like so:


$('[data-spy="scroll"]').each(function () {
  var $spy = $(this).scrollspy('refresh')
})

Options

Options can be passed via data attributes or JavaScript. For data attributes, append the option name to data-, as in data-offset="".
Name 	type 	default 	description
offset 	number 	10 	Pixels to offset from top when calculating position of scroll.
Events
Event Type 	Description
activate.bs.scrollspy 	This event fires whenever a new item becomes activated by the scrollspy.


$('#myScrollspy').on('activate.bs.scrollspy', function () {
  // do something…
})

Togglable tabs tab.js
Example tabs

Add quick, dynamic tab functionality to transition through panes of local content, even via dropdown menus. Nested tabs are not supported.

    Home
    Profile
    Dropdown

Raw denim you probably haven't heard of them jean shorts Austin. Nesciunt tofu stumptown aliqua, retro synth master cleanse. Mustache cliche tempor, williamsburg carles vegan helvetica. Reprehenderit butcher retro keffiyeh dreamcatcher synth. Cosby sweater eu banh mi, qui irure terry richardson ex squid. Aliquip placeat salvia cillum iphone. Seitan aliquip quis cardigan american apparel, butcher voluptate nisi qui.
Extends tabbed navigation

This plugin extends the tabbed navigation component to add tabbable areas.
Usage

Enable tabbable tabs via JavaScript (each tab needs to be activated individually):


$('#myTabs a').click(function (e) {
  e.preventDefault()
  $(this).tab('show')
})

You can activate individual tabs in several ways:


$('#myTabs a[href="#profile"]').tab('show') // Select tab by name
$('#myTabs a:first').tab('show') // Select first tab
$('#myTabs a:last').tab('show') // Select last tab
$('#myTabs li:eq(2) a').tab('show') // Select third tab (0-indexed)

Markup

You can activate a tab or pill navigation without writing any JavaScript by simply specifying data-toggle="tab" or data-toggle="pill" on an element. Adding the nav and nav-tabs classes to the tab ul will apply the Bootstrap tab styling, while adding the nav and nav-pills classes will apply pill styling.


<div>

  <!-- Nav tabs -->
  <ul class="nav nav-tabs" role="tablist">
    <li role="presentation" class="active"><a href="#home" aria-controls="home" role="tab" data-toggle="tab">Home</a></li>
    <li role="presentation"><a href="#profile" aria-controls="profile" role="tab" data-toggle="tab">Profile</a></li>
    <li role="presentation"><a href="#messages" aria-controls="messages" role="tab" data-toggle="tab">Messages</a></li>
    <li role="presentation"><a href="#settings" aria-controls="settings" role="tab" data-toggle="tab">Settings</a></li>
  </ul>

  <!-- Tab panes -->
  <div class="tab-content">
    <div role="tabpanel" class="tab-pane active" id="home">...</div>
    <div role="tabpanel" class="tab-pane" id="profile">...</div>
    <div role="tabpanel" class="tab-pane" id="messages">...</div>
    <div role="tabpanel" class="tab-pane" id="settings">...</div>
  </div>

</div>

Fade effect

To make tabs fade in, add .fade to each .tab-pane. The first tab pane must also have .in to make the initial content visible.


<div class="tab-content">
  <div role="tabpanel" class="tab-pane fade in active" id="home">...</div>
  <div role="tabpanel" class="tab-pane fade" id="profile">...</div>
  <div role="tabpanel" class="tab-pane fade" id="messages">...</div>
  <div role="tabpanel" class="tab-pane fade" id="settings">...</div>
</div>

Methods
$().tab

Activates a tab element and content container. Tab should have either a data-target or an href targeting a container node in the DOM. In the above examples, the tabs are the <a>s with data-toggle="tab" attributes.
.tab('show')

Selects the given tab and shows its associated content. Any other tab that was previously selected becomes unselected and its associated content is hidden. Returns to the caller before the tab pane has actually been shown (i.e. before the shown.bs.tab event occurs).


$('#someTab').tab('show')

Events

When showing a new tab, the events fire in the following order:

    hide.bs.tab (on the current active tab)
    show.bs.tab (on the to-be-shown tab)
    hidden.bs.tab (on the previous active tab, the same one as for the hide.bs.tab event)
    shown.bs.tab (on the newly-active just-shown tab, the same one as for the show.bs.tab event)

If no tab was already active, then the hide.bs.tab and hidden.bs.tab events will not be fired.
Event Type 	Description
show.bs.tab 	This event fires on tab show, but before the new tab has been shown. Use event.target and event.relatedTarget to target the active tab and the previous active tab (if available) respectively.
shown.bs.tab 	This event fires on tab show after a tab has been shown. Use event.target and event.relatedTarget to target the active tab and the previous active tab (if available) respectively.
hide.bs.tab 	This event fires when a new tab is to be shown (and thus the previous active tab is to be hidden). Use event.target and event.relatedTarget to target the current active tab and the new soon-to-be-active tab, respectively.
hidden.bs.tab 	This event fires after a new tab is shown (and thus the previous active tab is hidden). Use event.target and event.relatedTarget to target the previous active tab and the new active tab, respectively.


$('a[data-toggle="tab"]').on('shown.bs.tab', function (e) {
  e.target // newly activated tab
  e.relatedTarget // previous active tab
})

Tooltips tooltip.js

Inspired by the excellent jQuery.tipsy plugin written by Jason Frame; Tooltips are an updated version, which don't rely on images, use CSS3 for animations, and data-attributes for local title storage.

Tooltips with zero-length titles are never displayed.
Examples

Hover over the links below to see tooltips:

Tight pants next level keffiyeh you probably haven't heard of them. Photo booth beard raw denim letterpress vegan messenger bag stumptown. Farm-to-table seitan, mcsweeney's fixie sustainable quinoa 8-bit american apparel have a terry richardson vinyl chambray. Beard stumptown, cardigans banh mi lomo thundercats. Tofu biodiesel williamsburg marfa, four loko mcsweeney's cleanse vegan chambray. A really ironic artisan whatever keytar, scenester farm-to-table banksy Austin twitter handle freegan cred raw denim single-origin coffee viral.
Static tooltip

Four options are available: top, right, bottom, and left aligned.
Tooltip on the left
Tooltip on the top
Tooltip on the bottom
Tooltip on the right
Four directions


<button type="button" class="btn btn-default" data-toggle="tooltip" data-placement="left" title="Tooltip on left">Tooltip on left</button>

<button type="button" class="btn btn-default" data-toggle="tooltip" data-placement="top" title="Tooltip on top">Tooltip on top</button>

<button type="button" class="btn btn-default" data-toggle="tooltip" data-placement="bottom" title="Tooltip on bottom">Tooltip on bottom</button>

<button type="button" class="btn btn-default" data-toggle="tooltip" data-placement="right" title="Tooltip on right">Tooltip on right</button>

Opt-in functionality

For performance reasons, the Tooltip and Popover data-apis are opt-in, meaning you must initialize them yourself.

One way to initialize all tooltips on a page would be to select them by their data-toggle attribute:


$(function () {
  $('[data-toggle="tooltip"]').tooltip()
})

Usage

The tooltip plugin generates content and markup on demand, and by default places tooltips after their trigger element.

Trigger the tooltip via JavaScript:


$('#example').tooltip(options)

Markup

The required markup for a tooltip is only a data attribute and title on the HTML element you wish to have a tooltip. The generated markup of a tooltip is rather simple, though it does require a position (by default, set to top by the plugin).


<!-- HTML to write -->
<a href="#" data-toggle="tooltip" title="Some tooltip text!">Hover over me</a>

<!-- Generated markup by the plugin -->
<div class="tooltip top" role="tooltip">
  <div class="tooltip-arrow"></div>
  <div class="tooltip-inner">
    Some tooltip text!
  </div>
</div>

Multiple-line links

Sometimes you want to add a tooltip to a hyperlink that wraps multiple lines. The default behavior of the tooltip plugin is to center it horizontally and vertically. Add white-space: nowrap; to your anchors to avoid this.
Tooltips in button groups, input groups, and tables require special setting

When using tooltips on elements within a .btn-group or an .input-group, or on table-related elements (<td>, <th>, <tr>, <thead>, <tbody>, <tfoot>), you'll have to specify the option container: 'body' (documented below) to avoid unwanted side effects (such as the element growing wider and/or losing its rounded corners when the tooltip is triggered).
Don't try to show tooltips on hidden elements

Invoking $(...).tooltip('show') when the target element is display: none; will cause the tooltip to be incorrectly positioned.
Accessible tooltips for keyboard and assistive technology users

For users navigating with a keyboard, and in particular users of assistive technologies, you should only add tooltips to keyboard-focusable elements such as links, form controls, or any arbitrary element with a tabindex="0" attribute.
Tooltips on disabled elements require wrapper elements

To add a tooltip to a disabled or .disabled element, put the element inside of a <div> and apply the tooltip to that <div> instead.
Options

Options can be passed via data attributes or JavaScript. For data attributes, append the option name to data-, as in data-animation="".
Name 	Type 	Default 	Description
animation 	boolean 	true 	Apply a CSS fade transition to the tooltip
container 	string | false 	false 	

Appends the tooltip to a specific element. Example: container: 'body'. This option is particularly useful in that it allows you to position the tooltip in the flow of the document near the triggering element - which will prevent the tooltip from floating away from the triggering element during a window resize.
delay 	number | object 	0 	

Delay showing and hiding the tooltip (ms) - does not apply to manual trigger type

If a number is supplied, delay is applied to both hide/show

Object structure is: delay: { "show": 500, "hide": 100 }
html 	boolean 	false 	Insert HTML into the tooltip. If false, jQuery's text method will be used to insert content into the DOM. Use text if you're worried about XSS attacks.
placement 	string | function 	'top' 	

How to position the tooltip - top | bottom | left | right | auto.
When "auto" is specified, it will dynamically reorient the tooltip. For example, if placement is "auto left", the tooltip will display to the left when possible, otherwise it will display right.

When a function is used to determine the placement, it is called with the tooltip DOM node as its first argument and the triggering element DOM node as its second. The this context is set to the tooltip instance.
selector 	string 	false 	If a selector is provided, tooltip objects will be delegated to the specified targets. In practice, this is used to enable dynamic HTML content to have tooltips added. See this and an informative example.
template 	string 	'<div class="tooltip" role="tooltip"><div class="tooltip-arrow"></div><div class="tooltip-inner"></div></div>' 	

Base HTML to use when creating the tooltip.

The tooltip's title will be injected into the .tooltip-inner.

.tooltip-arrow will become the tooltip's arrow.

The outermost wrapper element should have the .tooltip class.
title 	string | function 	'' 	

Default title value if title attribute isn't present.

If a function is given, it will be called with its this reference set to the element that the tooltip is attached to.
trigger 	string 	'hover focus' 	How tooltip is triggered - click | hover | focus | manual. You may pass multiple triggers; separate them with a space. manual cannot be combined with any other trigger.
viewport 	string | object | function 	{ selector: 'body', padding: 0 } 	

Keeps the tooltip within the bounds of this element. Example: viewport: '#viewport' or { "selector": "#viewport", "padding": 0 }

If a function is given, it is called with the triggering element DOM node as its only argument. The this context is set to the tooltip instance.
Data attributes for individual tooltips

Options for individual tooltips can alternatively be specified through the use of data attributes, as explained above.
Methods
$().tooltip(options)

Attaches a tooltip handler to an element collection.
.tooltip('show')

Reveals an element's tooltip. Returns to the caller before the tooltip has actually been shown (i.e. before the shown.bs.tooltip event occurs). This is considered a "manual" triggering of the tooltip. Tooltips with zero-length titles are never displayed.


$('#element').tooltip('show')

.tooltip('hide')

Hides an element's tooltip. Returns to the caller before the tooltip has actually been hidden (i.e. before the hidden.bs.tooltip event occurs). This is considered a "manual" triggering of the tooltip.


$('#element').tooltip('hide')

.tooltip('toggle')

Toggles an element's tooltip. Returns to the caller before the tooltip has actually been shown or hidden (i.e. before the shown.bs.tooltip or hidden.bs.tooltip event occurs). This is considered a "manual" triggering of the tooltip.


$('#element').tooltip('toggle')

.tooltip('destroy')

Hides and destroys an element's tooltip. Tooltips that use delegation (which are created using the selector option) cannot be individually destroyed on descendant trigger elements.


$('#element').tooltip('destroy')

Events
Event Type 	Description
show.bs.tooltip 	This event fires immediately when the show instance method is called.
shown.bs.tooltip 	This event is fired when the tooltip has been made visible to the user (will wait for CSS transitions to complete).
hide.bs.tooltip 	This event is fired immediately when the hide instance method has been called.
hidden.bs.tooltip 	This event is fired when the tooltip has finished being hidden from the user (will wait for CSS transitions to complete).
inserted.bs.tooltip 	This event is fired after the show.bs.tooltip event when the tooltip template has been added to the DOM.


$('#myTooltip').on('hidden.bs.tooltip', function () {
  // do something…
})

Popovers popover.js

Add small overlays of content, like those on the iPad, to any element for housing secondary information.

Popovers whose both title and content are zero-length are never displayed.
Plugin dependency

Popovers require the tooltip plugin to be included in your version of Bootstrap.
Opt-in functionality

For performance reasons, the Tooltip and Popover data-apis are opt-in, meaning you must initialize them yourself.

One way to initialize all popovers on a page would be to select them by their data-toggle attribute:


$(function () {
  $('[data-toggle="popover"]').popover()
})

Popovers in button groups, input groups, and tables require special setting

When using popovers on elements within a .btn-group or an .input-group, or on table-related elements (<td>, <th>, <tr>, <thead>, <tbody>, <tfoot>), you'll have to specify the option container: 'body' (documented below) to avoid unwanted side effects (such as the element growing wider and/or losing its rounded corners when the popover is triggered).
Don't try to show popovers on hidden elements

Invoking $(...).popover('show') when the target element is display: none; will cause the popover to be incorrectly positioned.
Popovers on disabled elements require wrapper elements

To add a popover to a disabled or .disabled element, put the element inside of a <div> and apply the popover to that <div> instead.
Multiple-line links

Sometimes you want to add a popover to a hyperlink that wraps multiple lines. The default behavior of the popover plugin is to center it horizontally and vertically. Add white-space: nowrap; to your anchors to avoid this.
Examples
Static popover

Four options are available: top, right, bottom, and left aligned.
Popover top

Sed posuere consectetur est at lobortis. Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum.
Popover right

Sed posuere consectetur est at lobortis. Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum.
Popover bottom

Sed posuere consectetur est at lobortis. Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum.
Popover left

Sed posuere consectetur est at lobortis. Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum.
Live demo


<button type="button" class="btn btn-lg btn-danger" data-toggle="popover" title="Popover title" data-content="And here's some amazing content. It's very engaging. Right?">Click to toggle popover</button>

Four directions


<button type="button" class="btn btn-default" data-container="body" data-toggle="popover" data-placement="left" data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus.">
  Popover on left
</button>

<button type="button" class="btn btn-default" data-container="body" data-toggle="popover" data-placement="top" data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus.">
  Popover on top
</button>

<button type="button" class="btn btn-default" data-container="body" data-toggle="popover" data-placement="bottom" data-content="Vivamus
sagittis lacus vel augue laoreet rutrum faucibus.">
  Popover on bottom
</button>

<button type="button" class="btn btn-default" data-container="body" data-toggle="popover" data-placement="right" data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus.">
  Popover on right
</button>

Dismiss on next click

Use the focus trigger to dismiss popovers on the next click that the user makes.
Specific markup required for dismiss-on-next-click

For proper cross-browser and cross-platform behavior, you must use the <a> tag, not the <button> tag, and you also must include the role="button" and tabindex attributes.


<a tabindex="0" class="btn btn-lg btn-danger" role="button" data-toggle="popover" data-trigger="focus" title="Dismissible popover" data-content="And here's some amazing content. It's very engaging. Right?">Dismissible popover</a>

Usage

Enable popovers via JavaScript:


$('#example').popover(options)

Options

Options can be passed via data attributes or JavaScript. For data attributes, append the option name to data-, as in data-animation="".
Name 	Type 	Default 	Description
animation 	boolean 	true 	Apply a CSS fade transition to the popover
container 	string | false 	false 	

Appends the popover to a specific element. Example: container: 'body'. This option is particularly useful in that it allows you to position the popover in the flow of the document near the triggering element - which will prevent the popover from floating away from the triggering element during a window resize.
content 	string | function 	'' 	

Default content value if data-content attribute isn't present.

If a function is given, it will be called with its this reference set to the element that the popover is attached to.
delay 	number | object 	0 	

Delay showing and hiding the popover (ms) - does not apply to manual trigger type

If a number is supplied, delay is applied to both hide/show

Object structure is: delay: { "show": 500, "hide": 100 }
html 	boolean 	false 	Insert HTML into the popover. If false, jQuery's text method will be used to insert content into the DOM. Use text if you're worried about XSS attacks.
placement 	string | function 	'right' 	

How to position the popover - top | bottom | left | right | auto.
When "auto" is specified, it will dynamically reorient the popover. For example, if placement is "auto left", the popover will display to the left when possible, otherwise it will display right.

When a function is used to determine the placement, it is called with the popover DOM node as its first argument and the triggering element DOM node as its second. The this context is set to the popover instance.
selector 	string 	false 	If a selector is provided, popover objects will be delegated to the specified targets. In practice, this is used to enable dynamic HTML content to have popovers added. See this and an informative example.
template 	string 	'<div class="popover" role="tooltip"><div class="arrow"></div><h3 class="popover-title"></h3><div class="popover-content"></div></div>' 	

Base HTML to use when creating the popover.

The popover's title will be injected into the .popover-title.

The popover's content will be injected into the .popover-content.

.arrow will become the popover's arrow.

The outermost wrapper element should have the .popover class.
title 	string | function 	'' 	

Default title value if title attribute isn't present.

If a function is given, it will be called with its this reference set to the element that the popover is attached to.
trigger 	string 	'click' 	How popover is triggered - click | hover | focus | manual. You may pass multiple triggers; separate them with a space. manual cannot be combined with any other trigger.
viewport 	string | object | function 	{ selector: 'body', padding: 0 } 	

Keeps the popover within the bounds of this element. Example: viewport: '#viewport' or { "selector": "#viewport", "padding": 0 }

If a function is given, it is called with the triggering element DOM node as its only argument. The this context is set to the popover instance.
Data attributes for individual popovers

Options for individual popovers can alternatively be specified through the use of data attributes, as explained above.
Methods
$().popover(options)

Initializes popovers for an element collection.
.popover('show')

Reveals an element's popover. Returns to the caller before the popover has actually been shown (i.e. before the shown.bs.popover event occurs). This is considered a "manual" triggering of the popover. Popovers whose both title and content are zero-length are never displayed.


$('#element').popover('show')

.popover('hide')

Hides an element's popover. Returns to the caller before the popover has actually been hidden (i.e. before the hidden.bs.popover event occurs). This is considered a "manual" triggering of the popover.


$('#element').popover('hide')

.popover('toggle')

Toggles an element's popover. Returns to the caller before the popover has actually been shown or hidden (i.e. before the shown.bs.popover or hidden.bs.popover event occurs). This is considered a "manual" triggering of the popover.


$('#element').popover('toggle')

.popover('destroy')

Hides and destroys an element's popover. Popovers that use delegation (which are created using the selector option) cannot be individually destroyed on descendant trigger elements.


$('#element').popover('destroy')

Events
Event Type 	Description
show.bs.popover 	This event fires immediately when the show instance method is called.
shown.bs.popover 	This event is fired when the popover has been made visible to the user (will wait for CSS transitions to complete).
hide.bs.popover 	This event is fired immediately when the hide instance method has been called.
hidden.bs.popover 	This event is fired when the popover has finished being hidden from the user (will wait for CSS transitions to complete).
inserted.bs.popover 	This event is fired after the show.bs.popover event when the popover template has been added to the DOM.


$('#myPopover').on('hidden.bs.popover', function () {
  // do something…
})

Alert messages alert.js
Example alerts

Add dismiss functionality to all alert messages with this plugin.

When using a .close button, it must be the first child of the .alert-dismissible and no text content may come before it in the markup.
Holy guacamole! Best check yo self, you're not looking too good.
Oh snap! You got an error!

Change this and that and try again. Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem nec elit. Cras mattis consectetur purus sit amet fermentum.

Usage

Just add data-dismiss="alert" to your close button to automatically give an alert close functionality. Closing an alert removes it from the DOM.


<button type="button" class="close" data-dismiss="alert" aria-label="Close">
  <span aria-hidden="true">&times;</span>
</button>

To have your alerts use animation when closing, make sure they have the .fade and .in classes already applied to them.
Methods
$().alert()

Makes an alert listen for click events on descendant elements which have the data-dismiss="alert" attribute. (Not necessary when using the data-api's auto-initialization.)
$().alert('close')

Closes an alert by removing it from the DOM. If the .fade and .in classes are present on the element, the alert will fade out before it is removed.
Events

Bootstrap's alert plugin exposes a few events for hooking into alert functionality.
Event Type 	Description
close.bs.alert 	This event fires immediately when the close instance method is called.
closed.bs.alert 	This event is fired when the alert has been closed (will wait for CSS transitions to complete).


$('#myAlert').on('closed.bs.alert', function () {
  // do something…
})

Buttons button.js

Do more with buttons. Control button states or create groups of buttons for more components like toolbars.
Cross-browser compatibility

Firefox persists form control states (disabledness and checkedness) across page loads. A workaround for this is to use autocomplete="off". See Mozilla bug #654072.
Stateful

Add data-loading-text="Loading..." to use a loading state on a button.

This feature is deprecated since v3.3.5 and has been removed in v4.
Use whichever state you like!

For the sake of this demonstration, we are using data-loading-text and $().button('loading'), but that's not the only state you can use. See more on this below in the $().button(string) documentation.


<button type="button" id="myButton" data-loading-text="Loading..." class="btn btn-primary" autocomplete="off">
  Loading state
</button>

<script>
  $('#myButton').on('click', function () {
    var $btn = $(this).button('loading')
    // business logic...
    $btn.button('reset')
  })
</script>

Single toggle

Add data-toggle="button" to activate toggling on a single button.
Pre-toggled buttons need .active and aria-pressed="true"

For pre-toggled buttons, you must add the .active class and the aria-pressed="true" attribute to the button yourself.


<button type="button" class="btn btn-primary" data-toggle="button" aria-pressed="false" autocomplete="off">
  Single toggle
</button>

Checkbox / Radio

Add data-toggle="buttons" to a .btn-group containing checkbox or radio inputs to enable toggling in their respective styles.
Preselected options need .active

For preselected options, you must add the .active class to the input's label yourself.
Visual checked state only updated on click

If the checked state of a checkbox button is updated without firing a click event on the button (e.g. via <input type="reset"> or via setting the checked property of the input), you will need to toggle the .active class on the input's label yourself.


<div class="btn-group" data-toggle="buttons">
  <label class="btn btn-primary active">
    <input type="checkbox" autocomplete="off" checked> Checkbox 1 (pre-checked)
  </label>
  <label class="btn btn-primary">
    <input type="checkbox" autocomplete="off"> Checkbox 2
  </label>
  <label class="btn btn-primary">
    <input type="checkbox" autocomplete="off"> Checkbox 3
  </label>
</div>



<div class="btn-group" data-toggle="buttons">
  <label class="btn btn-primary active">
    <input type="radio" name="options" id="option1" autocomplete="off" checked> Radio 1 (preselected)
  </label>
  <label class="btn btn-primary">
    <input type="radio" name="options" id="option2" autocomplete="off"> Radio 2
  </label>
  <label class="btn btn-primary">
    <input type="radio" name="options" id="option3" autocomplete="off"> Radio 3
  </label>
</div>

Methods
$().button('toggle')

Toggles push state. Gives the button the appearance that it has been activated.
$().button('reset')

Resets button state - swaps text to original text. This method is asynchronous and returns before the resetting has actually completed.
$().button(string)

Swaps text to any data defined text state.


<button type="button" id="myStateButton" data-complete-text="finished!" class="btn btn-primary" autocomplete="off">
  ...
</button>

<script>
  $('#myStateButton').on('click', function () {
    $(this).button('complete') // button text will be "finished!"
  })
</script>

Collapse collapse.js

Flexible plugin that utilizes a handful of classes for easy toggle behavior.
Plugin dependency

Collapse requires the transitions plugin to be included in your version of Bootstrap.
Example

Click the buttons below to show and hide another element via class changes:

    .collapse hides content
    .collapsing is applied during transitions
    .collapse.in shows content

You can use a link with the href attribute, or a button with the data-target attribute. In both cases, the data-toggle="collapse" is required.



<a class="btn btn-primary" role="button" data-toggle="collapse" href="#collapseExample" aria-expanded="false" aria-controls="collapseExample">
  Link with href
</a>
<button class="btn btn-primary" type="button" data-toggle="collapse" data-target="#collapseExample" aria-expanded="false" aria-controls="collapseExample">
  Button with data-target
</button>
<div class="collapse" id="collapseExample">
  <div class="well">
    ...
  </div>
</div>

Accordion example

Extend the default collapse behavior to create an accordion with the panel component.
Collapsible Group Item #1
Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch. Food truck quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon tempor, sunt aliqua put a bird on it squid single-origin coffee nulla assumenda shoreditch et. Nihil anim keffiyeh helvetica, craft beer labore wes anderson cred nesciunt sapiente ea proident. Ad vegan excepteur butcher vice lomo. Leggings occaecat craft beer farm-to-table, raw denim aesthetic synth nesciunt you probably haven't heard of them accusamus labore sustainable VHS.
Collapsible Group Item #2
Collapsible Group Item #3


<div class="panel-group" id="accordion" role="tablist" aria-multiselectable="true">
  <div class="panel panel-default">
    <div class="panel-heading" role="tab" id="headingOne">
      <h4 class="panel-title">
        <a role="button" data-toggle="collapse" data-parent="#accordion" href="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
          Collapsible Group Item #1
        </a>
      </h4>
    </div>
    <div id="collapseOne" class="panel-collapse collapse in" role="tabpanel" aria-labelledby="headingOne">
      <div class="panel-body">
        Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch. Food truck quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon tempor, sunt aliqua put a bird on it squid single-origin coffee nulla assumenda shoreditch et. Nihil anim keffiyeh helvetica, craft beer labore wes anderson cred nesciunt sapiente ea proident. Ad vegan excepteur butcher vice lomo. Leggings occaecat craft beer farm-to-table, raw denim aesthetic synth nesciunt you probably haven't heard of them accusamus labore sustainable VHS.
      </div>
    </div>
  </div>
  <div class="panel panel-default">
    <div class="panel-heading" role="tab" id="headingTwo">
      <h4 class="panel-title">
        <a class="collapsed" role="button" data-toggle="collapse" data-parent="#accordion" href="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
          Collapsible Group Item #2
        </a>
      </h4>
    </div>
    <div id="collapseTwo" class="panel-collapse collapse" role="tabpanel" aria-labelledby="headingTwo">
      <div class="panel-body">
        Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch. Food truck quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon tempor, sunt aliqua put a bird on it squid single-origin coffee nulla assumenda shoreditch et. Nihil anim keffiyeh helvetica, craft beer labore wes anderson cred nesciunt sapiente ea proident. Ad vegan excepteur butcher vice lomo. Leggings occaecat craft beer farm-to-table, raw denim aesthetic synth nesciunt you probably haven't heard of them accusamus labore sustainable VHS.
      </div>
    </div>
  </div>
  <div class="panel panel-default">
    <div class="panel-heading" role="tab" id="headingThree">
      <h4 class="panel-title">
        <a class="collapsed" role="button" data-toggle="collapse" data-parent="#accordion" href="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
          Collapsible Group Item #3
        </a>
      </h4>
    </div>
    <div id="collapseThree" class="panel-collapse collapse" role="tabpanel" aria-labelledby="headingThree">
      <div class="panel-body">
        Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch. Food truck quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon tempor, sunt aliqua put a bird on it squid single-origin coffee nulla assumenda shoreditch et. Nihil anim keffiyeh helvetica, craft beer labore wes anderson cred nesciunt sapiente ea proident. Ad vegan excepteur butcher vice lomo. Leggings occaecat craft beer farm-to-table, raw denim aesthetic synth nesciunt you probably haven't heard of them accusamus labore sustainable VHS.
      </div>
    </div>
  </div>
</div>

It's also possible to swap out .panel-bodys with .list-groups.
Collapsible list group
Make expand/collapse controls accessible

Be sure to add aria-expanded to the control element. This attribute explicitly defines the current state of the collapsible element to screen readers and similar assistive technologies. If the collapsible element is closed by default, it should have a value of aria-expanded="false". If you've set the collapsible element to be open by default using the in class, set aria-expanded="true" on the control instead. The plugin will automatically toggle this attribute based on whether or not the collapsible element has been opened or closed.

Additionally, if your control element is targeting a single collapsible element – i.e. the data-target attribute is pointing to an id selector – you may add an additional aria-controls attribute to the control element, containing the id of the collapsible element. Modern screen readers and similar assistive technologies make use of this attribute to provide users with additional shortcuts to navigate directly to the collapsible element itself.
Usage

The collapse plugin utilizes a few classes to handle the heavy lifting:

    .collapse hides the content
    .collapse.in shows the content
    .collapsing is added when the transition starts, and removed when it finishes

These classes can be found in component-animations.less.
Via data attributes

Just add data-toggle="collapse" and a data-target to the element to automatically assign control of a collapsible element. The data-target attribute accepts a CSS selector to apply the collapse to. Be sure to add the class collapse to the collapsible element. If you'd like it to default open, add the additional class in.

To add accordion-like group management to a collapsible control, add the data attribute data-parent="#selector". Refer to the demo to see this in action.
Via JavaScript

Enable manually with:


$('.collapse').collapse()

Options

Options can be passed via data attributes or JavaScript. For data attributes, append the option name to data-, as in data-parent="".
Name 	type 	default 	description
parent 	selector 	false 	If a selector is provided, then all collapsible elements under the specified parent will be closed when this collapsible item is shown. (similar to traditional accordion behavior - this is dependent on the panel class)
toggle 	boolean 	true 	Toggles the collapsible element on invocation
Methods
.collapse(options)

Activates your content as a collapsible element. Accepts an optional options object.


$('#myCollapsible').collapse({
  toggle: false
})

.collapse('toggle')

Toggles a collapsible element to shown or hidden. Returns to the caller before the collapsible element has actually been shown or hidden (i.e. before the shown.bs.collapse or hidden.bs.collapse event occurs).
.collapse('show')

Shows a collapsible element. Returns to the caller before the collapsible element has actually been shown (i.e. before the shown.bs.collapse event occurs).
.collapse('hide')

Hides a collapsible element. Returns to the caller before the collapsible element has actually been hidden (i.e. before the hidden.bs.collapse event occurs).
Events

Bootstrap's collapse class exposes a few events for hooking into collapse functionality.
Event Type 	Description
show.bs.collapse 	This event fires immediately when the show instance method is called.
shown.bs.collapse 	This event is fired when a collapse element has been made visible to the user (will wait for CSS transitions to complete).
hide.bs.collapse 	This event is fired immediately when the hide method has been called.
hidden.bs.collapse 	This event is fired when a collapse element has been hidden from the user (will wait for CSS transitions to complete).


$('#myCollapsible').on('hidden.bs.collapse', function () {
  // do something…
})

Carousel carousel.js

A slideshow component for cycling through elements, like a carousel. Nested carousels are not supported.
Examples

First slide [900x500]
Previous
Next


<div id="carousel-example-generic" class="carousel slide" data-ride="carousel">
  <!-- Indicators -->
  <ol class="carousel-indicators">
    <li data-target="#carousel-example-generic" data-slide-to="0" class="active"></li>
    <li data-target="#carousel-example-generic" data-slide-to="1"></li>
    <li data-target="#carousel-example-generic" data-slide-to="2"></li>
  </ol>

  <!-- Wrapper for slides -->
  <div class="carousel-inner" role="listbox">
    <div class="item active">
      <img src="..." alt="...">
      <div class="carousel-caption">
        ...
      </div>
    </div>
    <div class="item">
      <img src="..." alt="...">
      <div class="carousel-caption">
        ...
      </div>
    </div>
    ...
  </div>

  <!-- Controls -->
  <a class="left carousel-control" href="#carousel-example-generic" role="button" data-slide="prev">
    <span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </a>
  <a class="right carousel-control" href="#carousel-example-generic" role="button" data-slide="next">
    <span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
  </a>
</div>

Accessibility issue

The carousel component is generally not compliant with accessibility standards. If you need to be compliant, please consider other options for presenting your content.
Transition animations not supported in Internet Explorer 8 & 9

Bootstrap exclusively uses CSS3 for its animations, but Internet Explorer 8 & 9 don't support the necessary CSS properties. Thus, there are no slide transition animations when using these browsers. We have intentionally decided not to include jQuery-based fallbacks for the transitions.
Initial active element required

The .active class needs to be added to one of the slides. Otherwise, the carousel will not be visible.
Glyphicon icons not necessary

The .glyphicon .glyphicon-chevron-left and .glyphicon .glyphicon-chevron-right classes are not necessarily needed for the controls. Bootstrap provides .icon-prev and .icon-next as plain unicode alternatives.
Optional captions

Add captions to your slides easily with the .carousel-caption element within any .item. Place just about any optional HTML within there and it will be automatically aligned and formatted.

900x500
First slide label

Nulla vitae elit libero, a pharetra augue mollis interdum.
Previous
Next


<div class="item">
  <img src="..." alt="...">
  <div class="carousel-caption">
    <h3>...</h3>
    <p>...</p>
  </div>
</div>

Usage
Multiple carousels

Carousels require the use of an id on the outermost container (the .carousel) for carousel controls to function properly. When adding multiple carousels, or when changing a carousel's id, be sure to update the relevant controls.
Via data attributes

Use data attributes to easily control the position of the carousel. data-slide accepts the keywords prev or next, which alters the slide position relative to its current position. Alternatively, use data-slide-to to pass a raw slide index to the carousel data-slide-to="2", which shifts the slide position to a particular index beginning with 0.

The data-ride="carousel" attribute is used to mark a carousel as animating starting at page load. It cannot be used in combination with (redundant and unnecessary) explicit JavaScript initialization of the same carousel.
Via JavaScript

Call carousel manually with:


$('.carousel').carousel()

Options

Options can be passed via data attributes or JavaScript. For data attributes, append the option name to data-, as in data-interval="".
Name 	type 	default 	description
interval 	number 	5000 	The amount of time to delay between automatically cycling an item. If false, carousel will not automatically cycle.
pause 	string | null 	"hover" 	If set to "hover", pauses the cycling of the carousel on mouseenter and resumes the cycling of the carousel on mouseleave. If set to null, hovering over the carousel won't pause it.
wrap 	boolean 	true 	Whether the carousel should cycle continuously or have hard stops.
keyboard 	boolean 	true 	Whether the carousel should react to keyboard events.
Methods
.carousel(options)

Initializes the carousel with an optional options object and starts cycling through items.


$('.carousel').carousel({
  interval: 2000
})

.carousel('cycle')

Cycles through the carousel items from left to right.
.carousel('pause')

Stops the carousel from cycling through items.
.carousel(number)

Cycles the carousel to a particular frame (0 based, similar to an array).
.carousel('prev')

Cycles to the previous item.
.carousel('next')

Cycles to the next item.
Events

Bootstrap's carousel class exposes two events for hooking into carousel functionality.

Both events have the following additional properties:

    direction: The direction in which the carousel is sliding (either "left" or "right").
    relatedTarget: The DOM element that is being slid into place as the active item.

All carousel events are fired at the carousel itself (i.e. at the <div class="carousel">).
Event Type 	Description
slide.bs.carousel 	This event fires immediately when the slide instance method is invoked.
slid.bs.carousel 	This event is fired when the carousel has completed its slide transition.


$('#myCarousel').on('slide.bs.carousel', function () {
  // do something…
})

Affix affix.js
Example

The affix plugin toggles position: fixed; on and off, emulating the effect found with position: sticky;. The subnavigation on the right is a live demo of the affix plugin.
Usage

Use the affix plugin via data attributes or manually with your own JavaScript. In both situations, you must provide CSS for the positioning and width of your affixed content.

Note: Do not use the affix plugin on an element contained in a relatively positioned element, such as a pulled or pushed column, due to a Safari rendering bug.
Positioning via CSS

The affix plugin toggles between three classes, each representing a particular state: .affix, .affix-top, and .affix-bottom. You must provide the styles, with the exception of position: fixed; on .affix, for these classes yourself (independent of this plugin) to handle the actual positions.

Here's how the affix plugin works:

    To start, the plugin adds .affix-top to indicate the element is in its top-most position. At this point no CSS positioning is required.
    Scrolling past the element you want affixed should trigger the actual affixing. This is where .affix replaces .affix-top and sets position: fixed; (provided by Bootstrap's CSS).
    If a bottom offset is defined, scrolling past it should replace .affix with .affix-bottom. Since offsets are optional, setting one requires you to set the appropriate CSS. In this case, add position: absolute; when necessary. The plugin uses the data attribute or JavaScript option to determine where to position the element from there.

Follow the above steps to set your CSS for either of the usage options below.
Via data attributes

To easily add affix behavior to any element, just add data-spy="affix" to the element you want to spy on. Use offsets to define when to toggle the pinning of an element.


<div data-spy="affix" data-offset-top="60" data-offset-bottom="200">
  ...
</div>

Via JavaScript

Call the affix plugin via JavaScript:


$('#myAffix').affix({
  offset: {
    top: 100,
    bottom: function () {
      return (this.bottom = $('.footer').outerHeight(true))
    }
  }
})

Options

Options can be passed via data attributes or JavaScript. For data attributes, append the option name to data-, as in data-offset-top="200".
Name 	type 	default 	description
offset 	number | function | object 	10 	Pixels to offset from screen when calculating position of scroll. If a single number is provided, the offset will be applied in both top and bottom directions. To provide a unique, bottom and top offset just provide an object offset: { top: 10 } or offset: { top: 10, bottom: 5 }. Use a function when you need to dynamically calculate an offset.
target 	selector | node | jQuery element 	the window object 	Specifies the target element of the affix.
Methods
.affix(options)

Activates your content as affixed content. Accepts an optional options object.


$('#myAffix').affix({
  offset: 15
})

.affix('checkPosition')

Recalculates the state of the affix based on the dimensions, position, and scroll position of the relevant elements. The .affix, .affix-top, and .affix-bottom classes are added to or removed from the affixed content according to the new state. This method needs to be called whenever the dimensions of the affixed content or the target element are changed, to ensure correct positioning of the affixed content.


$('#myAffix').affix('checkPosition')

Events

Bootstrap's affix plugin exposes a few events for hooking into affix functionality.
Event Type 	Description
affix.bs.affix 	This event fires immediately before the element has been affixed.
affixed.bs.affix 	This event is fired after the element has been affixed.
affix-top.bs.affix 	This event fires immediately before the element has been affixed-top.
affixed-top.bs.affix 	This event is fired after the element has been affixed-top.
affix-bottom.bs.affix 	This event fires immediately before the element has been affixed-bottom.
affixed-bottom.bs.affix 	This event is fired after the element has been affixed-bottom.
-------------------------------------------------------------------------------

-------------------------------------------------------------------------------
