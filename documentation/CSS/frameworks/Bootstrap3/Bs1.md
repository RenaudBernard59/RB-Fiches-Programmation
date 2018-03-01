# Bootstrap

## I-Presentation

[LINK](https://getbootstrap.com/docs/3.3/)

**Bootstrap is the most popular HTML, CSS, and JS framework for developing responsive, mobile first projects on the web.**

*Currently v3.3.7*

### A-Designed for everyone, everywhere

Bootstrap makes front-end web development faster and easier. It's made for folks of all skill levels, devices of all shapes, and projects of all sizes.
Sass and Less support

#### 1-Preprocessors

Bootstrap ships with vanilla CSS, but its source code utilizes the two most popular CSS preprocessors, Less and Sass. Quickly get started with precompiled CSS or build on the source.
Responsive across devices

#### 2-One framework, every device.

Bootstrap easily and efficiently scales your websites and applications with a single code base, from phones to tablets to desktops with CSS media queries.
Components

#### 3-Full of features

With Bootstrap, you get extensive and beautiful documentation for common HTML elements, dozens of custom HTML and CSS components, and awesome jQuery plugins.

*Bootstrap is open source. It's hosted, developed, and maintained on GitHub.*

[Github](https://github.com/twbs/bootstrap)

### B-Official Bootstrap Themes

Take Bootstrap to the next level with official premium themes. Each theme is its own toolkit featuring all of Bootstrap, brand new components and plugins, full docs, build tools, and more.

[Browse themes](https://themes.getbootstrap.com/)

### C-Built with Bootstrap

Millions of amazing sites across the web are being built with Bootstrap. Get started on your own with our growing [collection of examples](https://getbootstrap.com/docs/getting-started/#examples) or by exploring some of our favorites.

* [Lyft](http://expo.getbootstrap.com/2014/10/29/lyft/)
* [Vogue](https://getbootstrap.com/assets/img/expo-vogue.jpg)
* [Riot Design](https://getbootstrap.com/assets/img/expo-riot.jpg)
* [Newsweek](http://expo.getbootstrap.com/2014/02/12/newsweek/)

We showcase dozens of inspiring projects built with Bootstrap on the Bootstrap Expo.

[Explore the Exop](http://expo.getbootstrap.com/)

-------------------------------------------------------------------------------

## II-Getting started

[LINK](https://getbootstrap.com/docs/3.3/getting-started/)

**An overview of Bootstrap, how to download and use, basic templates and examples, and more.**

### A-Download

Bootstrap (currently v3.3.7) has a few easy ways to quickly get started, each one appealing to a different skill level and use case. Read through to see what suits your particular needs.

##### a-Bootstrap

Compiled and minified CSS, JavaScript, and fonts. No docs or original source files are included.

[Download](https://github.com/twbs/bootstrap/releases/download/v3.3.7/bootstrap-3.3.7-dist.zip)

##### b-Source code

Source Less, JavaScript, and font files, along with our docs. Requires a Less compiler and some setup.

[Download](https://github.com/twbs/bootstrap/archive/v3.3.7.zip)

##### c-Sass

Bootstrap ported from Less to Sass for easy inclusion in Rails, Compass, or Sass-only projects.

[Download](https://github.com/twbs/bootstrap-sass/archive/v3.3.7.tar.gz)

#### 1-Bootstrap CDN

The folks over at [MaxCDN](https://www.maxcdn.com/) graciously provide CDN support for Bootstrap's CSS and JavaScript. Just use these [Bootstrap CDN](https://www.bootstrapcdn.com/) links.


        ```html
    <!-- Latest compiled and minified CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">

    <!-- Optional theme -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap-theme.min.css" integrity="sha384-rHyoN1iRsVXV4nD0JutlnGaslCJuC7uwjduW9SVrLvRYooPp2bWYgmgJQIXwl/Sp" crossorigin="anonymous">

    <!-- Latest compiled and minified JavaScript -->
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js" integrity="sha384-Tc5IQib027qvyjSMfHjOMaLkfuWVxZxUPnCJA7l2mCWNIpG9mGCD8wGNIcPD7Txa" crossorigin="anonymous"></script>
    ```

#### 2-Install with Bower

You can also install and manage Bootstrap's Less, CSS, JavaScript, and fonts using [Bower](http://bower.io/):

        ```shel
    $ bower install bootstrap
    ```

#### 3-Install with npm

You can also install Bootstrap using [npm](https://www.npmjs.com/):

        ```shel
    $ npm install bootstrap@3
    ```

`require('bootstrap')` will load all of Bootstrap's jQuery plugins onto the jQuery object. The `bootstrap` module itself does not export anything. You can manually load Bootstrap's jQuery plugins individually by loading the **/js/*.js** files under the package's top-level directory.

Bootstrap's `package.json` contains some additional metadata under the following keys:

* `less` - path to Bootstrap's main [Less](http://lesscss.org/) source file
* `style` - path to Bootstrap's non-minified CSS that's been precompiled using the default settings (no customization)

#### 4-Install with Composer

You can also install and manage Bootstrap's Less, CSS, JavaScript, and fonts using [Composer](https://getcomposer.org/):

        ```shel
    $ composer require twbs/bootstrap
    ```

#### 5-Autoprefixer required for Less/Sass

Bootstrap uses [Autoprefixer](https://github.com/postcss/autoprefixer) to deal with [CSS vendor prefixes](http://webdesign.about.com/od/css/a/css-vendor-prefixes.htm). If you're compiling Bootstrap from its Less/Sass source and not using our Gruntfile, you'll need to integrate Autoprefixer into your build process yourself. If you're using precompiled Bootstrap or using our Gruntfile, you don't need to worry about this because Autoprefixer is already integrated into our Gruntfile.

### B-What's included

**Bootstrap is downloadable in two forms, within which you'll find the following directories and files, logically grouping common resources and providing both compiled and minified variations.**

> **jQuery required**
>
>> Please note that *all JavaScript plugins require jQuery* to be included, as shown in the [starter template](https://getbootstrap.com/docs/3.3/getting-started/#template). Consult our **bower.json** to see which versions of jQuery are supported.

#### 1-Precompiled Bootstrap

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

#### 2-Bootstrap source code

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

### C-Compiling CSS and JavaScript

**Bootstrap uses [Grunt](http://gruntjs.com/) for its build system, with convenient methods for working with the framework. It's how we compile our code, run tests, and more.**

#### 1-Installing Grunt

To install Grunt, you must first download and [install node.js](https://nodejs.org/download/) (which includes npm). npm stands for [node packaged modules](https://www.npmjs.com/) and is a way to manage development dependencies through node.js.
Then, from the command line:

1. Install `grunt-cli` globally with `npm install -g grunt-cli`.
2. Navigate to the root `/bootstrap/` directory, then run `npm install`. npm will look at the `package.json` file and automatically install the necessary local dependencies listed there.

When completed, you'll be able to run the various Grunt commands provided from the command line.

#### 2-Available Grunt commands

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

#### 3-Troubleshooting

Should you encounter problems with installing dependencies or running Grunt commands, first delete the `/node_modules/` directory generated by npm. Then, rerun npm install.

### D-Basic template

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

### E-Examples

**Build on the basic template above with Bootstrap's many components. We encourage you to customize and adapt Bootstrap to suit your individual project's needs.**

Get the source code for every example below by [downloading the Bootstrap repository](https://github.com/twbs/bootstrap/archive/v3.3.7.zip). Examples can be found in the `docs/examples/ directory`.

#### 1-Using the framework

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

#### 2-Navbars in action

![Navbar example]()

**Navbar**

Super basic template that includes the navbar along with some additional content.

![Static top navbar example]()

**Static top navbar**

Super basic template with a static top navbar along with some additional content.

![Fixed navbar example]()

**Fixed navbar**

Super basic template with a fixed top navbar along with some additional content.

#### 3-Custom components

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

#### 4-Experiments

![Non-responsive example]()

**Non-responsive Bootstrap**

Easily disable the responsiveness of Bootstrap per our docs.

![Off-canvas navigation example]()

**Off-canvas**

Build a toggleable off-canvas navigation menu for use with Bootstrap.

### F-Tools

#### 1-Bootlint

**[Bootlint](https://github.com/twbs/bootlint)** is the official Bootstrap HTML [linter](http://en.wikipedia.org/wiki/Lint_(software)) tool. It automatically checks for several common HTML mistakes in webpages that are using Bootstrap in a fairly "vanilla" way. Vanilla Bootstrap's components/widgets require their parts of the DOM to conform to certain structures. Bootlint checks that instances of Bootstrap components have correctly-structured HTML. Consider adding Bootlint to your Bootstrap web development toolchain so that none of the common mistakes slow down your project's development.

### G-Community

**Stay up to date on the development of Bootstrap and reach out to the community with these helpful resources.**

* Read and subscribe to [The Official Bootstrap Blog](http://blog.getbootstrap.com/).
* Chat with fellow Bootstrappers using IRC in the `irc.freenode.net` server, in the [##bootstrap channel](irc://irc.freenode.net/%23bootstrap).
* For help using Bootstrap, ask on [StackOverflow using the tag](https://stackoverflow.com/questions/tagged/twitter-bootstrap-3) `twitter-bootstrap-3`.
* Developers should use the keyword `bootstrap` on packages which modify or add to the functionality of Bootstrap when distributing through [npm](https://www.npmjs.com/browse/keyword/bootstrap) or similar delivery mechanisms for maximum discoverability.
* Find inspiring examples of people building with Bootstrap at the [Bootstrap Expo](http://expo.getbootstrap.com/).

You can also follow [@getbootstrap on Twitter](https://twitter.com/getbootstrap) for the latest gossip and awesome music videos.

### H-Disabling responsiveness

**Bootstrap automatically adapts your pages for various screen sizes. Here's how to disable this feature so your page works like [this non-responsive example](https://getbootstrap.com/docs/3.3/examples/non-responsive/).**

#### 1-Steps to disable page responsiveness

1. Omit the viewport `<meta>` mentioned in [the CSS docs](https://getbootstrap.com/docs/3.3/css/#overview-mobile)
2. Override the `width` on the `.container` for each grid tier with a single `width, for example width: 970px !important;` Be sure that this comes after the default Bootstrap CSS. You can optionally avoid the `!important` with media queries or some selector-fu.
3. If using navbars, remove all navbar collapsing and expanding behavior.
4. For grid layouts, use `.col-xs-*` classes in addition to, or in place of, the medium/large ones. Don't worry, the extra-small device grid scales to all resolutions.

You'll still need Respond.js for IE8 (since our media queries are still there and need to be processed). This disables the "mobile site" aspects of Bootstrap.

#### 2-Bootstrap template with responsiveness disabled

We've applied these steps to an example. Read its source code to see the specific changes implemented.

[View non-responsive example](https://getbootstrap.com/docs/3.3/examples/non-responsive/)

>**Migrating from v2.x to v3.x**
>
>>Looking to migrate from an older version of Bootstrap to v3.x? Check [out our migration guide](https://getbootstrap.com/docs/3.3/migration).

### I-Browser and device support

**Bootstrap is built to work best in the latest desktop and mobile browsers, meaning older browsers might display differently styled, though fully functional, renderings of certain components.**

#### 1-Supported browsers

Specifically, we support the **latest versions** of the following browsers and platforms.

Alternative browsers which use the latest version of WebKit, Blink, or Gecko, whether directly or via the platform's web view API, are not explicitly supported. However, Bootstrap should (in most cases) display and function correctly in these browsers as well. More specific support information is provided below.

##### a-Mobile devices

Generally speaking, Bootstrap supports the latest versions of each major platform's default browsers. Note that proxy browsers (such as Opera Mini, Opera Mobile's Turbo mode, UC Browser Mini, Amazon Silk) are not supported.

| | Chrome | Firefox | Safari |
|------|------|------|------| 
| Android | Supported | Supported | N/A |
| iOS | Supported | Supported | Supported |

##### b-Desktop browsers

Similarly, the latest versions of most desktop browsers are supported.

| | Chrome | Firefox | Internet Explorer | Opera | Safari |
|------|------|------|------|------|------| 
| Mac | Supported | Supported | N/A | Supported | Supported |
| Windows | Supported | Supported | Supported | Supported | Not supported |

On Windows, **we support Internet Explorer 8-11**.

For Firefox, in addition to the latest normal stable release, we also support the latest [Extended Support Release (ESR)](https://www.mozilla.org/en-US/firefox/organizations/faq/) version of Firefox.

Unofficially, Bootstrap should look and behave well enough in Chromium and Chrome for Linux, Firefox for Linux, and Internet Explorer 7, as well as Microsoft Edge, though they are not officially supported.

For a list of some of the browser bugs that Bootstrap has to grapple with, see our [Wall of browser bugs](https://getbootstrap.com/docs/3.3/browser-bugs/).

#### 2-Internet Explorer 8 and 9

Internet Explorer 8 and 9 are also supported, however, please be aware that some CSS3 properties and HTML5 elements are not fully supported by these browsers. In addition, **Internet Explorer 8 requires the use of [Respond.js](https://github.com/scottjehl/Respond) to enable media query support**.

| Feature | Internet Explorer 8 | Internet Explorer 9 |
|------|------|------|
| `border-radius` | Not supported | Supported |
| `box-shadow` | Not supported | Supported |
| `transform` | Not supported | Supported, with `-ms` prefix |
| `transition` | Not supported |
| `placeholder` | Not supported |

Visit [Can I use...](http://caniuse.com/) for details on browser support of CSS3 and HTML5 features.

#### 3-Internet Explorer 8 and Respond.js

Beware of the following caveats when using Respond.js in your development and production environments for Internet Explorer 8.

##### a-Respond.js and cross-domain CSS

Using Respond.js with CSS hosted on a different (sub)domain (for example, on a CDN) requires some additional setup. [See the Respond.js docs](https://github.com/scottjehl/Respond/blob/master/README.md#cdnx-domain-setup) for details.

##### b-Respond.js and `file://`

Due to browser security rules, Respond.js doesn't work with pages viewed via the `file://` protocol (like when opening a local HTML file). To test responsive features in IE8, view your pages over HTTP(S). [See the Respond.js docs](https://github.com/scottjehl/Respond/blob/master/README.md#support--caveats) for details.

##### c-Respond.js and `@import`

Respond.js doesn't work with CSS that's referenced via `@import`. In particular, some Drupal configurations are known to use @import. [See the Respond.js docs](https://github.com/scottjehl/Respond/blob/master/README.md#support--caveats) for details.

#### 4-Internet Explorer 8 and box-sizing

IE8 does not fully support `box-sizing: border-box;` when combined with `min-width`, `max-width`, `min-height`, or `max-height`. For that reason, as of v3.0.1, we no longer use `max-width` on `.containers`.

#### 5-Internet Explorer 8 and @font-face

IE8 has some issues with `@font-face` when combined with `:before.` Bootstrap uses that combination with its Glyphicons. If a page is cached, and loaded without the mouse over the window (i.e. hit the refresh button or load something in an iframe) then the page gets rendered before the font loads. Hovering over the page (body) will show some of the icons and hovering over the remaining icons will show those as well. [See issue #13863](https://github.com/twbs/bootstrap/issues/13863) for details.

#### 6-IE Compatibility modes

Bootstrap is not supported in the old Internet Explorer compatibility modes. To be sure you're using the latest rendering mode for IE, consider including the appropriate `<meta>` tag in your pages:

    ```html
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    ```

Confirm the document mode by opening the debugging tools: press **[F12]** and check the "Document Mode".

This tag is included in all of Bootstrap's documentation and examples to ensure the best rendering possible in each supported version of Internet Explorer.

See [this StackOverflow question](https://stackoverflow.com/questions/6771258/whats-the-difference-if-meta-http-equiv-x-ua-compatible-content-ie-edge) for more information.

#### 7-Internet Explorer 10 in Windows 8 and Windows Phone 8

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

#### 8-Safari percent rounding

The rendering engine of versions of Safari prior to v7.1 for OS X and Safari for iOS v8.0 had some trouble with the number of decimal places used in our `.col-*-1` grid classes. So if you had 12 individual grid columns, you'd notice that they came up short compared to other rows of columns. Besides upgrading Safari/iOS, you have some options for workarounds:

* Add `.pull-right` to your last grid column to get the hard-right alignment
* Tweak your percentages manually to get the perfect rounding for Safari (more difficult than the first option)

#### 9-Modals, navbars, and virtual keyboards

##### a-Overflow and scrolling

Support for `overflow: hidden` on the `<body>` element is quite limited in iOS and Android. To that end, when you scroll past the top or bottom of a modal in either of those devices' browsers, the `<body>` content will begin to scroll. See [Crome bug #175502](https://bugs.chromium.org/p/chromium/issues/detail?id=175502) (fixed in Chrome v40) and [WebKit bug #153852](https://bugs.webkit.org/show_bug.cgi?id=153852).

##### b-iOS text fields and scrolling

As of iOS 9.3, while a modal is open, if the initial touch of a scroll gesture is within the boundary of a textual `<input>` or a `<textarea>`, the `<body>` content underneath the modal will be scrolled instead of the modal itself. See [WebKit bug #153856](https://bugs.webkit.org/show_bug.cgi?id=153856).

##### c-Virtual keyboards

Also, note that if you're using a fixed navbar or using inputs within a modal, iOS has a rendering bug that doesn't update the position of fixed elements when the virtual keyboard is triggered. A few workarounds for this include transforming your elements to `position: absolute` or invoking a timer on focus to try to correct the positioning manually. This is not handled by Bootstrap, so it is up to you to decide which solution is best for your application.

##### d-Navbar Dropdowns

The `.dropdown-backdrop` element isn't used on iOS in the nav because of the complexity of z-indexing. Thus, to close dropdowns in navbars, you must directly click the dropdown element (or [any other element which will fire a click event in iOS](https://developer.mozilla.org/en-US/docs/Web/Events/click#Safari_Mobile)).

#### 10-Browser zooming

Page zooming inevitably presents rendering artifacts in some components, both in Bootstrap and the rest of the web. Depending on the issue, we may be able to fix it (search first and then open an issue if need be). However, we tend to ignore these as they often have no direct solution other than hacky workarounds.

#### 11-Sticky `:hover`/`:focus` on mobile

Even though real hovering isn't possible on most touchscreens, most mobile browsers emulate hovering support and make `:hover` "sticky". In other words, `:hover` styles start applying after tapping an element and only stop applying after the user taps some other element. This can cause Bootstrap's `:hover` states to become undesirably "stuck" on such browsers. Some mobile browsers also make `:focus` similarly sticky. There is currently no simple workaround for these issues other than removing such styles entirely.

#### 12-Printing

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

#### 13-Android stock browser

Out of the box, Android 4.1 (and even some newer releases apparently) ship with the Browser app as the default web browser of choice (as opposed to Chrome). Unfortunately, the Browser app has lots of bugs and inconsistencies with CSS in general.

##### a-Select menus

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

#### 14-Validators

In order to provide the best possible experience to old and buggy browsers, Bootstrap uses [CSS browser hacks](http://browserhacks.com/) in several places to target special CSS to certain browser versions in order to work around bugs in the browsers themselves. These hacks understandably cause CSS validators to complain that they are invalid. In a couple places, we also use bleeding-edge CSS features that aren't yet fully standardized, but these are used purely for progressive enhancement.

These validation warnings don't matter in practice since the non-hacky portion of our CSS does fully validate and the hacky portions don't interfere with the proper functioning of the non-hacky portion, hence why we deliberately ignore these particular warnings.

Our HTML docs likewise have some trivial and inconsequential HTML validation warnings due to our inclusion of a workaround for [a certain Firefox bug](https://bugzilla.mozilla.org/show_bug.cgi?id=654072).

### H-Third party support

**While we don't officially support any third party plugins or add-ons, we do offer some useful advice to help avoid potential issues in your projects.**

#### 1-Box-sizing

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

### I-Accessibility

**Bootstrap follows common web standards and—with minimal extra effort—can be used to create sites that are accessible to those using AT.**

#### 1-Skip navigation

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

#### 2-Nested headings

When nesting headings (`<h1>` - `<h6>`), your primary document header should be an `<h1>`. Subsequent headings should make logical use of `<h2>` - `<h6>` such that screen readers can construct a table of contents for your pages.

Learn more at [HTML CodeSniffer](http://squizlabs.github.io/HTML_CodeSniffer/Standards/Section508/) and [Penn State's AccessAbility](http://accessibility.psu.edu/headings).

#### 3-Color contrast

Currently, some of the default color combinations available in Bootstrap (such as the various styled button classes, some of the code highlighting colors used for [basic code blocks](https://getbootstrap.com/docs/3.3/css/#code-block), the `.bg-primary` [contextual background](https://getbootstrap.com/docs/3.3/css/#helper-classes-backgrounds) helper class, and the default link color when used on a white background) have a low contrast ratio (below the [recommended ratio of 4.5:1](http://www.w3.org/TR/WCAG20/#visual-audio-contrast-contrast)). This can cause problems to users with low vision or who are color blind. These default colors may need to be modified to increase their contrast and legibility.

#### 4-Additional resources

* ["HTML Codesniffer" bookmarklet for identifying accessibility issues](https://github.com/squizlabs/HTML_CodeSniffer)
* [Chrome's Accessibility Developer Tools extension](https://chrome.google.com/webstore/detail/accessibility-developer-t/fpkknkljclfencbdbgkenhalefipecmb?hl=en)
* [Colour Contrast Analyser](http://www.paciellogroup.com/resources/contrastanalyser/)
* [The A11Y Project](http://a11yproject.com/)
* [MDN accessibility documentation](https://developer.mozilla.org/en-US/docs/Accessibility)

### J-License FAQs

**Bootstrap is released under the MIT license and is right 2016 Twitter. Boiled down to smaller chunks, it can be described with the following conditions.**

#### 1-It requires you to:

* Keep the license and right notice included in Bootstrap's CSS and JavaScript files when you use them in your works

#### 2-It permits you to:

* Freely download and use Bootstrap, in whole or in part, for personal, private, company internal, or commercial purposes
* Use Bootstrap in packages or distributions that you create
* Modify the source code
* Grant a sublicense to modify and distribute Bootstrap to third parties not included in the license

#### 3-It forbids you to:

* Hold the authors and license owners liable for damages as Bootstrap is provided without warranty
* Hold the creators or right holders of Bootstrap liable
* Redistribute any piece of Bootstrap without proper attribution
* Use any marks owned by Twitter in any way that might state or imply that Twitter endorses your distribution
* Use any marks owned by Twitter in any way that might state or imply that you created the Twitter software in question

#### 4-It does not require you to:

* Include the source of Bootstrap itself, or of any modifications you may have made to it, in any redistribution you may assemble that includes it
* Submit changes that you make to Bootstrap back to the Bootstrap project (though such feedback is encouraged)

The full Bootstrap license is located [in the project repository](https://github.com/twbs/bootstrap/blob/master/LICENSE) for more information.

### K-Translations

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