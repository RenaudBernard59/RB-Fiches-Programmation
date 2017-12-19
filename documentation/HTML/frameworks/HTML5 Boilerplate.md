HTML5 Boilerplate
Usage
Once you have cloned or downloaded HTML5 Boilerplate, creating a site or app usually involves the following:
1.	Set up the basic structure of the site.
2.	Add some content, style, and functionality.
3.	Run your site locally to see how it looks.
4.	(Optionally run a build script to automate the optimization of your site - e.g. ant build script)
5.	Deploy your site.
Basic structure
A basic HTML5 Boilerplate site initially looks something like this:
.
├── css
│   ├── main.css
│   └── normalize.css
├── doc
├── img
├── js
│   ├── main.js
│   ├── plugins.js
│   └── vendor
│       ├── jquery.min.js
│       └── modernizr.min.js
├── .editorconfig
├── .htaccess
├── 404.html
├── apple-touch-icon.png
├── browserconfig.xml
├── index.html
├── humans.txt
├── robots.txt
├── crossdomain.xml
├── favicon.ico
├── tile-wide.png
└── tile.png

What follows is a general overview of each major part and how to use them.
css
This directory should contain all your project's CSS files. It includes some initial CSS to help get you started from a solid foundation. About the CSS.
doc
This directory contains all the HTML5 Boilerplate documentation. You can use it as the location and basis for your own project's documentation.
js
This directory should contain all your project's JS files. Libraries, plugins, and custom code can all be included here. It includes some initial JS to help get you started. About the JavaScript.
.htaccess
The default web server configs are for Apache. For more information, please refer to the Apache Server Configs repository.
Host your site on a server other than Apache? You're likely to find the corresponding server configs project listed in our Server Configs repository.
404.html
A helpful custom 404 to get you started.
browserconfig.xml
This file contains all settings regarding custom tiles for IE11.
For more info on this topic, please refer to MSDN.
.editorconfig
The .editorconfig file is provided in order to encourage and help you and your team to maintain consistent coding styles between different editors and IDEs. Read more about the .editorconfig file.
index.html
This is the default HTML skeleton that should form the basis of all pages on your site. If you are using a server-side templating framework, then you will need to integrate this starting HTML with your setup.
Make sure that you update the URLs for the referenced CSS and JavaScript if you modify the directory structure at all.
If you are using Google Universal Analytics, make sure that you edit the corresponding snippet at the bottom to include your analytics ID.
humans.txt
Edit this file to include the team that worked on your site/app, and the technology powering it.
robots.txt
Edit this file to include any pages you need hidden from search engines.
crossdomain.xml
A template for working with cross-domain requests. About crossdomain.xml.
Icons
Replace the default favicon.ico, tile.png, tile-wide.png and Apple Touch Icon with your own.
If you want to use different Apple Touch Icons for different resolutions please refer to the according documentation.
You might want to check out Hans' handy HTML5 Boilerplate Favicon and Apple Touch Icon PSD-Template.

Frequently asked questions
●	Why is the Google Analytics code at the bottom? Google recommends it be placed in the <head>.
●	How can I integrate Bootstrap with HTML5 Boilerplate?
●	Do I need to upgrade my site each time a new version of HTML5 Boilerplate is released?
●	Where can I get help with support questions?
--
Why is the Google Analytics code at the bottom? Google recommends it be placed in the <head>.
The main advantage of placing it in the <head> is that you will track the user's pageview even if they leave the page before it has been fully loaded. However, having the code at the bottom of the page helps improve performance.
How can I integrate Bootstrap with HTML5 Boilerplate?
One simple way is to use Initializr and create a custom build that includes both HTML5 Boilerplate and Bootstrap.
Read more about how HTML5 Boilerplate and Bootstrap complement each other.
Do I need to upgrade my site each time a new version of HTML5 Boilerplate is released?
No, same as you don't normally replace the foundation of a house once it was built. However, there is nothing stopping you from trying to work in the latest changes, but you'll have to assess the costs/benefits of doing so.
Where can I get help with support questions?
Please ask for help on StackOverflow.
The HTML
By default, HTML5 Boilerplate provides two html pages:
●	index.html - a default HTML skeleton that should form the basis of all pages on your website
●	404.html - a placeholder 404 error page
index.html
The no-js class
The no-js class is provided in order to allow you to more easily and explicitly add custom styles based on whether JavaScript is disabled (.no-js) or enabled (.js). Using this technique also helps avoid the FOUC.
Language attribute
Please consider specifying the language of your content by adding the lang attribute to <html> as in this example:
<html class="no-js" lang="en">
The order of the <title> and <meta> tags
The order in which the <title> and the <meta> tags are specified is important because:
1.	the charset declaration (<meta charset="utf-8">):
○	must be included completely within the first 1024 bytes of the document
○	should be specified as early as possible (before any content that could be controlled by an attacker, such as a <title> element) in order to avoid a potential encoding-related security issue in Internet Explorer
2.	the meta tag for compatibility mode (<meta http-equiv="x-ua-compatible" content="ie=edge">):
○	needs to be included before all other tags except for the <title> and the other <meta> tags
x-ua-compatible
Internet Explorer 8/9/10 support document compatibility modes that affect the way webpages are interpreted and displayed. Because of this, even if your site's visitor is using, let's say, Internet Explorer 9, it's possible that IE will not use the latest rendering engine, and instead, decide to render your page using the Internet Explorer 5.5 rendering engine.
Specifying the x-ua-compatible meta tag:
<meta http-equiv="x-ua-compatible" content="ie=edge">
or sending the page with the following HTTP response header
X-UA-Compatible: IE=edge

will force Internet Explorer 8/9/10 to render the webpage in the highest available mode in the various cases when it may not, and therefore, ensure that anyone browsing your site is treated to the best possible user experience that browser can offer.
If possible, we recommend that you remove the meta tag and send only the HTTP response header as the meta tag will not always work if your site is served on a non-standard port, as Internet Explorer's preference option Display intranet sites in Compatibility View is checked by default.
If you are using Apache as your webserver, including the .htaccess file takes care of the HTTP header. If you are using a different server, check out our other server config.
Starting with Internet Explorer 11, document modes are deprecated. If your business still relies on older web apps and services that were designed for older versions of Internet Explorer, you might want to consider enabling Enterprise Mode throughout your company.
Mobile viewport
There are a few different options that you can use with the viewport meta tag. You can find out more in the Apple developer docs. HTML5 Boilerplate comes with a simple setup that strikes a good balance for general use cases.
<meta name="viewport" content="width=device-width, initial-scale=1">
Favicons and Touch Icon
The shortcut icons should be put in the root directory of your site. HTML5 Boilerplate comes with a default set of icons (include favicon and one Apple Touch Icon) that you can use as a baseline to create your own.
Please refer to the more detailed description in the Extend section of these docs.
Modernizr
HTML5 Boilerplate uses a custom build of Modernizr.
Modernizr is a JavaScript library which adds classes to the html element based on the results of feature test and which ensures that all browsers can make use of HTML5 elements (as it includes the HTML5 Shiv). This allows you to target parts of your CSS and JavaScript based on the features supported by a browser.
In general, in order to keep page load times to a minimum, it's best to call any JavaScript at the end of the page because if a script is slow to load from an external server it may cause the whole page to hang. That said, the Modernizr script needs to run before the browser begins rendering the page, so that browsers lacking support for some of the new HTML5 elements are able to handle them properly. Therefore the Modernizr script is the only JavaScript file synchronously loaded at the top of the document.
What about polyfills?
If you need to include polyfills in your project, you must make sure those load before any other JavaScript. If you're using some polyfill CDN service, like cdn.polyfill.io, just put it before the other scripts in the bottom of the page:
   <script src="https://cdn.polyfill.io/v1/polyfill.min.js"></script>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.2/jquery.min.js"></script>
    <script>window.jQuery || document.write('<script src="js/vendor/jquery-1.11.2.min.js"><\/script>')</script>
    <script src="js/plugins.js"></script>
    <script src="js/main.js"></script>
</body>
If you like to just include the polyfills yourself, you could include them in js/plugins.js. When you have a bunch of polyfills to load in, you could also create a polyfills.js file in the js/vendor directory. Also using this technique, make sure the polyfills are all loaded before any other Javascript.
There are some misconceptions about Modernizr and polyfills. It's important to understand that Modernizr just handles feature checking, not polyfilling itself. The only thing Modernizr does regarding polyfills is that the team maintains a huge list of cross Browser polyfills.
The content area
The central part of the boilerplate template is pretty much empty. This is intentional, in order to make the boilerplate suitable for both web page and web app development.
Browser Upgrade Prompt
The main content area of the boilerplate includes a prompt to install an up to date browser for users of IE 6/7. If you intended to support IE 6/7, then you should remove the snippet of code.
jQuery CDN for jQuery
The jQuery CDN version of the jQuery JavaScript library is referenced towards the bottom of the page. A local fallback of jQuery is included for rare instances when the CDN version might not be available, and to facilitate offline development.
The jQuery CDN version was chosen over other potential candidates (like Google's Hosted Libraries) because it's fast (comparable or faster than Google by some measures) and, (unlike Google's CDN) is available to China's hundreds of millions of internet users. For many years we chose the Google Hosted version over the jQuery CDN because it was available over HTTPS (the jQuery CDN was not,) and it offered a better chance of hitting the cache lottery owing to the popularity of the Google CDN. The first issue is no longer valid and the second is far outweighed by being able to serve jQuery to Chinese users.
While the jQuery CDN is a strong default solution your site or application may require a different configuration. Testing your site with services like WebPageTest and browser tools like PageSpeed Insights or YSlow will help you examine the real world performance of your site and can show where you can optimize your specific site or application.
Google Universal Analytics Tracking Code
Finally, an optimized version of the Google Universal Analytics tracking code is included. Google recommends that this script be placed at the top of the page. Factors to consider: if you place this script at the top of the page, you’ll be able to count users who don’t fully load the page, and you’ll incur the max number of simultaneous connections of the browser.
Further information:
●	Optimizing the Google Universal Analytics Snippet
●	Introduction to Analytics.js
●	Google Analytics Demos & Tools
N.B. The Google Universal Analytics snippet is included by default mainly because Google Analytics is currently one of the most popular tracking solutions out there. However, its usage isn't set in stone, and you SHOULD consider exploring thealternatives and use whatever suits your needs best!

The CSS
HTML5 Boilerplate's CSS includes:
●	Normalize.css
●	Useful defaults
●	Common helpers
●	Placeholder media queries
●	Print styles
This starting CSS does not rely on the presence of conditional class names, conditional style sheets, or Modernizr, and it is ready to use no matter what your development preferences happen to be.
Normalize.css
In order to make browsers render all elements more consistently and in line with modern standards, we includeNormalize.css — a modern, HTML5-ready alternative to CSS resets.
As opposed to CSS resets, Normalize.css:
●	targets only the styles that need normalizing
●	preserves useful browser defaults rather than erasing them
●	corrects bugs and common browser inconsistencies
●	improves usability with subtle improvements
●	doesn't clutter the debugging tools
●	has better documentation
For more information about Normalize.css, please refer to its project page, as well as this blog post.
Useful defaults
Several base styles are included that build upon Normalize.css. These styles:
●	provide basic typography settings that improve text readability
●	protect against unwanted text-shadow during text highlighting
●	tweak the default alignment of some elements (e.g.: img, video, fieldset, textarea)
●	style the prompt that is displayed to users using an outdated browser
You are free and even encouraged to modify or add to these base styles as your project requires.
Common helpers
Along with the base styles, we also provide some commonly used helper classes.
.hidden
The hidden class can be added to any element that you want to hide visually and from screen readers. It could be an element that will be populated and displayed later, or an element you will hide with JavaScript.
.visuallyhidden
The visuallyhidden class can be added to any element that you want to hide visually, while still have its content accessible to screen readers.
See also:
●	CSS in Action: Invisible Content Just for Screen Reader Users
●	Hiding content for accessibility
●	HTML5 Boilerplate - Issue #194.
.invisible
The invisible class can be added to any element that you want to hide visually and from screen readers, but without affecting the layout.
As opposed to the hidden class that effectively removes the element from the layout, the invisible class will simply make the element invisible while keeping it in the flow and not affecting the positioning of the surrounding content.
N.B. Try to stay away from, and don't use the classes specified above for keyword stuffing as you will harm your site's ranking!
.clearfix
The clearfix class can be added to any element to ensure that it always fully contains its floated children.
Over the years there have been many variants of the clearfix hack, but currently, we use the micro clearfix.
Media Queries
HTML5 Boilerplate makes it easy for you to get started with a mobile first and responsive web design approach to development. But it's worth remembering that there are no silver bullets.
We include placeholder media queries to help you build up your mobile styles for wider viewports and high-resolution displays. It's recommended that you adapt these media queries based on the content of your site rather than mirroring the fixed dimensions of specific devices.
If you do not want to take the mobile first approach, you can simply edit or remove these placeholder media queries. One possibility would be to work from wide viewports down, and use max-width media queries instead (e.g.: @media only screen and (max-width: 480px)).
For more features that can help you in your mobile web development, take a look into our Mobile Boilerplate.
Print styles
Lastly, we provide some useful print styles that will optimize the printing process, as well as make the printed pages easier to read.
At printing time, these styles will:
●	strip all background colors, change the font color to black, and remove the text-shadow — done in order to help save printer ink and speed up the printing process
●	underline and expand links to include the URL — done in order to allow users to know where to refer to
●	(exceptions to this are: the links that are fragment identifiers, or use the javascript: pseudo protocol)
●	expand abbreviations to include the full description — done in order to allow users to know what the abbreviations stands for
●	provide instructions on how browsers should break the content into pages and on orphans/widows, namely, we instructsupporting browsers that they should:
○	ensure the table header (<thead>) is printed on each page spanned by the table
○	prevent block quotations, preformatted text, images and table rows from being split onto two different pages
○	ensure that headings never appear on a different page than the text they are associated with
○	ensure that orphans and widows do not appear on printed pages
The print styles are included along with the other css to avoid the additional HTTP request. Also, they should always be included last, so that the other styles can be overwritten.
The JavaScript
Information about the default JavaScript included in the project.
main.js
This file can be used to contain or reference your site/app JavaScript code. For larger projects, you can make use of a JavaScript module loader, like Require.js, to load any other scripts you need to run.
plugins.js
This file can be used to contain all your plugins, such as jQuery plugins and other 3rd party scripts.
One approach is to put jQuery plugins inside of a (function($){ ... })(jQuery); closure to make sure they're in the jQuery namespace safety blanket. Read more about jQuery plugin authoring.
By default the plugins.js file contains a small script to avoid console errors in browsers that lack a console. The script will make sure that, if a console method isn't available, that method will have the value of empty function, thus, preventing the browser from throwing an error.
vendor
This directory can be used to contain all 3rd party library code.
Minified versions of the latest jQuery and Modernizr libraries are included by default. You may wish to create your own custom Modernizr build.
Miscellaneous
●	.gitignore
●	.editorconfig
●	Server Configuration
●	crossdomain.xml
●	robots.txt
●	browserconfig.xml
--
.gitignore
HTML5 Boilerplate includes a basic project-level .gitignore. This should primarily be used to avoid certain project-level files and directories from being kept under source control. Different development-environments will benefit from different collections of ignores.
OS-specific and editor-specific files should be ignored using a "global ignore" that applies to all repositories on your system.
For example, add the following to your ~/.gitconfig, where the .gitignore in your HOME directory contains the files and directories you'd like to globally ignore:
[core]
    excludesfile = ~/.gitignore

●	More on global ignores: https://help.github.com/articles/ignoring-files
●	Comprehensive set of ignores on GitHub: https://github.com/github/gitignore
.editorconfig
The .editorconfig file is provided in order to encourage and help you and your team define and maintain consistent coding styles between different editors and IDEs.
By default, .editorconfig includes some basic properties that reflect the coding styles from the files provided by default, but you can easily change them to better suit your needs.
In order for your editor/IDE to apply the properties from the .editorconfig file, you will need to install a plugin.
N.B. If you aren't using the server configurations provided by HTML5 Boilerplate, we highly encourage you to configure your server to block access to .editorconfig files, as they can disclose sensitive information!
For more details, please refer to the EditorConfig project.
Server Configuration
H5BP includes a .htaccess file for the Apache HTTP server. If you are not using Apache as your web server, then you are encouraged to download a server configuration that corresponds to your web server and environment.
A .htaccess (hypertext access) file is a Apache HTTP server configuration file. The .htaccess file is mostly used for:
●	Rewriting URLs
●	Controlling cache
●	Authentication
●	Server-side includes
●	Redirects
●	Gzipping
If you have access to the main server configuration file (usually called httpd.conf), you should add the logic from the .htaccess file in, for example, a section in the main configuration file. This is usually the recommended way, as using .htaccess files slows down Apache!
To enable Apache modules locally, please see: https://github.com/h5bp/server-configs-apache/wiki/How-to-enable-Apache-modules.
In the repo the .htaccess is used for:
●	Allowing cross-origin access to web fonts
●	CORS header for images when browsers request it
●	Enable 404.html as 404 error document
●	Making the website experience better for IE users better
●	Media UTF-8 as character encoding for text/html and text/plain
●	Enabling the rewrite URLs engine
●	Forcing or removing the www. at the begin of a URL
●	It blocks access to directories without a default document
●	It blocks access to files that can expose sensitive information.
●	It reduces MIME type security risks
●	It forces compressing (gzipping)
●	It tells the browser whether they should request a specific file from the server or whether they should grab it from the browser's cache
When using .htaccess we recommend reading all inline comments (the rules after a #) in the file once. There is a bunch of optional stuff in it.
If you want to know more about the .htaccess file check out the Apache HTTP server docs or more specifically the htaccess section.
Notice that the original repo for the .htaccess file is this one.
crossdomain.xml
The cross-domain policy file is an XML document that gives a web client — such as Adobe Flash Player, Adobe Reader, etc. — permission to handle data across multiple domains, by:
●	granting read access to data
●	permitting the client to include custom headers in cross-domain requests
●	granting permissions for socket-based connections
e.g. If a client hosts content from a particular source domain and that content makes requests directed towards a domain other than its own, the remote domain would need to host a cross-domain policy file in order to grant access to the source domain and allow the client to continue with the transaction.
For more in-depth information, please see Adobe's cross-domain policy file specification.
robots.txt
The robots.txt file is used to give instructions to web robots on what can be crawled from the website.
By default, the file provided by this project includes the next two lines:
●	User-agent: * - the following rules apply to all web robots
●	Disallow: - everything on the website is allowed to be crawled
If you want to disallow certain pages you will need to specify the path in a Disallow directive (e.g.: Disallow: /path) or, if you want to disallow crawling of all content, use Disallow: /.
The /robots.txt file is not intended for access control, so don't try to use it as such. Think of it as a "No Entry" sign, rather than a locked door. URLs disallowed by the robots.txt file might still be indexed without being crawled, and the content from within the robots.txt file can be viewed by anyone, potentially disclosing the location of your private content! So, if you want to block access to private content, use proper authentication instead.
For more information about robots.txt, please see:
●	robotstxt.org
●	How Google handles the robots.txt file
browserconfig.xml
The browserconfig.xml file is used to customize the tile displayed when users pin your site to the Windows 8.1 start screen. In there you can define custom tile colors, custom images or even live tiles.
By default, the file points to 2 placeholder tile images:
●	tile.png (558x558px): used for Small, Medium and Large tiles. This image resizes automatically when necessary.
●	tile-wide.png (558x270px): user for Wide tiles.
Notice that IE11 uses the same images when adding a site to the favorites.
For more in-depth information about the browserconfig.xml file, please see MSDN.
Extend and customise HTML5 Boilerplate
Here is some useful advice for how you can make your project with HTML5 Boilerplate even better. We don't want to include it all by default, as not everything fits with everyone's needs.
●	App Stores
●	DNS prefetching
●	Google Universal Analytics
●	Internet Explorer
●	Miscellaneous
●	News Feeds
●	Search
●	Social Networks
●	URLs
●	Web Apps
App Stores
Install a Chrome Web Store app
Users can install a Chrome app directly from your website, as long as the app and site have been associated via Google's Webmaster Tools. Read more on Chrome Web Store's Inline Installation docs.
<link rel="chrome-webstore-item" href="https://chrome.google.com/webstore/detail/APP_ID">
Smart App Banners in iOS 6+ Safari
Stop bothering everyone with gross modals advertising your entry in the App Store. Include the following meta tag will unintrusively allow the user the option to download your iOS app, or open it with some data about the user's current state on the website.
<meta name="apple-itunes-app" content="app-id=APP_ID,app-argument=SOME_TEXT">
DNS prefetching
In short, DNS Prefetching is a method of informing the browser of domain names referenced on a site so that the client can resolve the DNS for those hosts, cache them, and when it comes time to use them, have a faster turn around on the request.
Implicit prefetches
There is a lot of prefetching done for you automatically by the browser. When the browser encounters an anchor in your html that does not share the same domain name as the current location the browser requests, from the client OS, the IP address for this new domain. The client first checks its cache and then, lacking a cached copy, makes a request from a DNS server. These requests happen in the background and are not meant to block the rendering of the page.
The goal of this is that when the foreign IP address is finally needed it will already be in the client cache and will not block the loading of the foreign content. Fewer requests result in faster page load times. The perception of this is increased on a mobile platform where DNS latency can be greater.
Disable implicit prefetching
<meta http-equiv="x-dns-prefetch-control" content="off">
Even with X-DNS-Prefetch-Control meta tag (or http header) browsers will still prefetch any explicit dns-prefetch links.
WARNING: THIS MAY MAKE YOUR SITE SLOWER IF YOU RELY ON RESOURCES FROM FOREIGN DOMAINS.
Explicit prefetches
Typically the browser only scans the HTML for foreign domains. If you have resources that are outside of your HTML (a javascript request to a remote server or a CDN that hosts content that may not be present on every page of your site, for example) then you can queue up a domain name to be prefetched.
<link rel="dns-prefetch" href="//example.com">
<link rel="dns-prefetch" href="https://ajax.googleapis.com">
You can use as many of these as you need, but it's best if they are all immediately after the Meta Charset element (which should go right at the top of the head), so the browser can act on them ASAP.
Common Prefetch Links
Amazon S3:
<link rel="dns-prefetch" href="//s3.amazonaws.com">
Google APIs:
<link rel="dns-prefetch" href="https://ajax.googleapis.com">
Microsoft Ajax Content Delivery Network:
<link rel="dns-prefetch" href="//ajax.microsoft.com">
<link rel="dns-prefetch" href="//ajax.aspnetcdn.com">
Further reading about DNS prefetching
●	https://developer.mozilla.org/en-US/docs/Controlling_DNS_prefetching
●	https://dev.chromium.org/developers/design-documents/dns-prefetching
●	http://blogs.msdn.com/b/ie/archive/2011/03/17/internet-explorer-9-network-performance-improvements.aspx
●	http://dayofjs.com/videos/22158462/web-browsers_alex-russel
Google Universal Analytics
More tracking settings
The optimized Google Universal Analytics snippet included with HTML5 Boilerplate includes something like this:
ga('create', 'UA-XXXXX-X', 'auto'); ga('send', 'pageview');
To customize further, see Google's Advanced Setup, Pageview, and Event Docs.
Anonymize IP addresses
In some countries, no personal data may be transferred outside jurisdictions that do not have similarly strict laws (i.e. from Germany to outside the EU). Thus a webmaster using the Google Universal Analytics may have to ensure that no personal (trackable) data is transferred to the US. You can do that with the ga('set', 'anonymizeIp', true); parameter before sending any events/pageviews. In use it looks like this:
ga('create', 'UA-XXXXX-X', 'auto');
ga('set', 'anonymizeIp', true);
ga('send', 'pageview');
Track jQuery AJAX requests in Google Analytics
An article by @JangoSteve explains how to track jQuery AJAX requests in Google Analytics.
Add this to plugins.js:
/*
 * Log all jQuery AJAX requests to Google Analytics
 * See: http://www.alfajango.com/blog/track-jquery-ajax-requests-in-google-analytics/
 */
if (typeof ga !== "undefined" && ga !== null) {
    $(document).ajaxSend(function(event, xhr, settings){
        ga('send', 'pageview', settings.url);
    });
}
Track JavaScript errors in Google Analytics
Add this function after ga is defined:
(function(window){
    var undefined,
        link = function (href) {
            var a = window.document.createElement('a');
            a.href = href;
            return a;
        };
    window.onerror = function (message, file, line, column) {
        var host = link(file).hostname;
        ga('send', {
          'hitType': 'event',
          'eventCategory': (host == window.location.hostname || host == undefined || host == '' ? '' : 'external ') + 'error',
          'eventAction': message,
          'eventLabel': (file + ' LINE: ' + line + (column ? ' COLUMN: ' + column : '')).trim(),
          'nonInteraction': 1
        });
    };
}(window));
Track page scroll
Add this function after ga is defined:
$(function(){
    var isDuplicateScrollEvent,
        scrollTimeStart = new Date,
        $window = $(window),
        $document = $(document),
        scrollPercent;

    $window.scroll(function() {
        scrollPercent = Math.round(100 * ($window.height() + $window.scrollTop())/$document.height());
        if (scrollPercent > 90 && !isDuplicateScrollEvent) { //page scrolled to 90%
            isDuplicateScrollEvent = 1;
            ga('send', 'event', 'scroll',
                'Window: ' + $window.height() + 'px; Document: ' + $document.height() + 'px; Time: ' + Math.round((new Date - scrollTimeStart )/1000,1) + 's'
            );
        }
    });
});
Internet Explorer
Prompt users to switch to "Desktop Mode" in IE10 Metro
IE10 does not support plugins, such as Flash, in Metro mode. If your site requires plugins, you can let users know that via thex-ua-compatible meta element, which will prompt them to switch to Desktop Mode.
<meta http-equiv="x-ua-compatible" content="requiresActiveX=true">
Here's what it looks like alongside H5BP's default x-ua-compatible values:
<meta http-equiv="x-ua-compatible" content="ie=edge,requiresActiveX=true">
You can find more information in Microsoft's IEBlog post about prompting for plugin use in IE10 Metro Mode.
IE Pinned Sites (IE9+)
Enabling your application for pinning will allow IE9 users to add it to their Windows Taskbar and Start Menu. This comes with a range of new tools that you can easily configure with the elements below. See more documentation on IE9 Pinned Sites.
Name the Pinned Site for Windows
Without this rule, Windows will use the page title as the name for your application.
<meta name="application-name" content="Sample Title">
Give your Pinned Site a tooltip
You know — a tooltip. A little textbox that appears when the user holds their mouse over your Pinned Site's icon.
<meta name="msapplication-tooltip" content="A description of what this site does.">
Set a default page for your Pinned Site
If the site should go to a specific URL when it is pinned (such as the homepage), enter it here. One idea is to send it to a special URL so you can track the number of pinned users, like so: http://www.example.com/index.html?pinned=true
<meta name="msapplication-starturl" content="http://www.example.com/index.html?pinned=true">
Recolor IE's controls manually for a Pinned Site
IE9+ will automatically use the overall color of your Pinned Site's favicon to shade its browser buttons. UNLESS you give it another color here. Only use named colors (red) or hex colors (#ff0000).
<meta name="msapplication-navbutton-color" content="#ff0000">
Manually set the window size of a Pinned Site
If the site should open at a certain window size once pinned, you can specify the dimensions here. It only supports static pixel dimensions. 800x600 minimum.
<meta name="msapplication-window" content="width=800;height=600">
Jump List "Tasks" for Pinned Sites
Add Jump List Tasks that will appear when the Pinned Site's icon gets a right-click. Each Task goes to the specified URL, and gets its own mini icon (essentially a favicon, a 16x16 .ICO). You can add as many of these as you need.
<meta name="msapplication-task" content="name=Task 1;action-uri=http://host/Page1.html;icon-uri=http://host/icon1.ico">
<meta name="msapplication-task" content="name=Task 2;action-uri=http://microsoft.com/Page2.html;icon-uri=http://host/icon2.ico">
(Windows 8) High quality visuals for Pinned Sites
Windows 8 adds the ability for you to provide a PNG tile image and specify the tile's background color. Full details on the IE blog.
●	Create a 144x144 image of your site icon, filling all of the canvas, and using a transparent background.
●	Save this image as a 32-bit PNG and optimize it without reducing colour-depth. It can be named whatever you want (e.g. metro-tile.png).
●	To reference the tile and its color, add the HTML meta elements described in the IE Blog post.
(Windows 8) Badges for Pinned Sites
IE10 will poll an XML document for badge information to display on your app's tile in the Start screen. The user will be able to receive these badge updates even when your app isn't actively running. The badge's value can be a number, or one of a predefined list of glyphs.
●	Tutorial on IEBlog with link to badge XML schema
●	Available badge values
<meta name="msapplication-badge" value="frequency=NUMBER_IN_MINUTES;polling-uri=http://www.example.com/path/to/file.xml">
Disable link highlighting upon tap in IE10
Similar to -webkit-tap-highlight-color in iOS Safari. Unlike that CSS property, this is an HTML meta element, and its value is boolean rather than a color. It's all or nothing.
<meta name="msapplication-tap-highlight" content="no" />
You can read about this useful element and more techniques in Microsoft's documentation on adapting WebKit-oriented apps for IE10
Search
Direct search spiders to your sitemap
Learn how to make a sitemap
<link rel="sitemap" type="application/xml" title="Sitemap" href="/sitemap.xml">
Hide pages from search engines
According to Heather Champ, former community manager at Flickr, you should not allow search engines to index your "Contact Us" or "Complaints" page if you value your sanity. This is an HTML-centric way of achieving that.
<meta name="robots" content="noindex">
WARNING: DO NOT INCLUDE ON PAGES THAT SHOULD APPEAR IN SEARCH ENGINES.
Firefox and IE Search Plugins
Sites with in-site search functionality should be strongly considered for a browser search plugin. A "search plugin" is an XML file which defines how your plugin behaves in the browser. How to make a browser search plugin.
<link rel="search" title="" type="application/opensearchdescription+xml" href="">
Miscellaneous
●	Use polyfills.
●	Use Microformats (via microdata) for optimum search results visibility.
●	If you're building a web app you may want native style momentum scrolling in iOS 5+ using -webkit-overflow-scrolling: touch.
●	If you want to disable the translation prompt in Chrome or block Google Translate from translating your web page, use <meta name="google" value="notranslate">. To disable translation for a particular section of the web page, addclass="notranslate".
●	If you want to disable the automatic detection and formatting of possible phone numbers in Safari on iOS, use <meta name="format-detection" content="telephone=no">.
●	Avoid development/stage websites "leaking" into SERPs (search engine results page) by implementing X-Robots-tag headers.
●	Screen readers currently have less-than-stellar support for HTML5 but the JS script accessifyhtml5.js can help increase accessibility by adding ARIA roles to HTML5 elements.
News Feeds
RSS
Have an RSS feed? Link to it here. Want to learn how to write an RSS feed from scratch?
<link rel="alternate" type="application/rss+xml" title="RSS" href="/rss.xml">
Atom
Atom is similar to RSS, and you might prefer to use it instead of or in addition to it. See what Atom's all about.
<link rel="alternate" type="application/atom+xml" title="Atom" href="/atom.xml">
Pingbacks
Your server may be notified when another site links to yours. The href attribute should contain the location of your pingback service.
<link rel="pingback" href="">
●	High-level explanation: https://codex.wordpress.org/Introduction_to_Blogging#Pingbacks
●	Step-by-step example case: http://www.hixie.ch/specs/pingback/pingback-1.0#TOC5
●	PHP pingback service: https://web.archive.org/web/20131211032834/http://blog.perplexedlabs.com/2009/07/15/xmlrpc-pingbacks-using-php/
Social Networks
Facebook Open Graph data
You can control the information that Facebook and others display when users share your site. Below are just the most basic data points you might need. For specific content types (including "website"), see Facebook's built-in Open Graph content templates. Take full advantage of Facebook's support for complex data and activity by following the Open Graph tutorial.
<meta property="og:title" content="">
<meta property="og:description" content="">
<meta property="og:image" content="">
Twitter Cards
Twitter provides a snippet specification that serves a similar purpose to Open Graph. In fact, Twitter will use Open Graph when Cards is not available. Note that, as of this writing, Twitter requires that app developers activate Cards on a per-domain basis. You can read more about the various snippet formats and application process in the official Twitter Cards documentation.
<meta name="twitter:card" content="summary">
<meta name="twitter:site" content="@site_account">
<meta name="twitter:creator" content="@individual_account">
<meta name="twitter:url" content="http://www.example.com/path/to/page.html">
<meta name="twitter:title" content="">
<meta name="twitter:description" content="">
<meta name="twitter:image" content="http://www.example.com/path/to/image.jpg">
URLs
Canonical URL
Signal to search engines and others "Use this URL for this page!" Useful when parameters after a # or ? is used to control the display state of a page. http://www.example.com/cart.html?shopping-cart-open=true can be indexed as the cleaner, more accurate http://www.example.com/cart.html.
<link rel="canonical" href="">
Official shortlink
Signal to the world "This is the shortened URL to use this page!" Poorly supported at this time. Learn more by reading the article about shortlinks on the Microformats wiki.
<link rel="shortlink" href="h5bp.com">
Separate mobile URLs
If you use separate URLs for desktop and mobile users, you should consider helping search engine algorithms better understand the configuration on your web site.
This can be done by adding the following annotations in your HTML pages:
●	on the desktop page, add the link rel="alternate" tag pointing to the corresponding mobile URL, e.g.:
●	<link rel="alternate" media="only screen and (max-width: 640px)" href="http://m.example.com/page.html" >
●	on the mobile page, add the link rel="canonical" tag pointing to the corresponding desktop URL, e.g.:
●	<link rel="canonical" href="http://www.example.com/page.html">
For more information please see:
●	https://developers.google.com/webmasters/smartphone-sites/details#separateurls
●	https://developers.google.com/webmasters/smartphone-sites/feature-phones
Web Apps
There are a couple of meta tags that provide information about a web app when added to the Home Screen on iOS:
●	Adding apple-mobile-web-app-capable will make your web app chrome-less and provide the default iOS app view. You can control the color scheme of the default view by adding apple-mobile-web-app-status-bar-style.
```
●	You can use apple-mobile-web-app-title to add a specific sites name for the Home Screen icon. This works since iOS 6.
```
For further information please read the official documentation on Apple's site.
Apple Touch Icons
The Apple touch icons can be seen as the favicons of iOS devices.
The main sizes of the Apple touch icons are:
●	57×57px – iPhone with @1x display and iPod Touch
●	72×72px – iPad and iPad mini with @1x display running iOS ≤ 6
●	76×76px – iPad and iPad mini with @1x display running iOS ≥ 7
●	114×114px – iPhone with @2x display running iOS ≤ 6
●	120×120px – iPhone with @2x and @3x display running iOS ≥ 7
●	144×144px – iPad and iPad mini with @2x display running iOS ≤ 6
●	152×152px – iPad and iPad mini with @2x display running iOS 7
●	180×180px – iPad and iPad mini with @2x display running iOS 8
Displays meaning:
●	@1x - non-Retina
●	@2x - Retina
●	@3x - Retina HD
More information about the displays of iOS devices can be found here.
In most cases, one 180×180px touch icon named apple-touch-icon.png and including:
<link rel="apple-touch-icon" href="apple-touch-icon.png">
in the <head> of the page is enough. If you use art-direction and/or want to have different content for each device, you can add more touch icons as written above.
For a more comprehensive overview, please refer to Mathias' article on Touch Icons.
Apple Touch Startup Image
Apart from that it is possible to add start-up screens for web apps on iOS. This basically works by defining apple-touch-startup-image with an according link to the image. Since iOS devices have different screen resolutions it is necessary to add media queries to detect which image to load. Here is an example for a retina iPhone:
<link rel="apple-touch-startup-image" media="(max-device-width: 480px) and (-webkit-min-device-pixel-ratio: 2)" href="img/startup-retina.png">
However, it is possible to detect which start-up image to use with JavaScript. The Mobile Boilerplate provides a useful function for this. Please see helpers.js for the implementation.
Chrome Mobile web apps
Chrome Mobile has a specific meta tag for making apps installable to the homescreen which tries to be a more generic replacement to Apple's proprietary meta tag:
<meta name="mobile-web-app-capable" content="yes">
Same applies to the touch icons:
<link rel="icon" sizes="192x192" href="highres-icon.png">
Theme Color
You can add the theme-color meta extension in the <head> of your pages to suggest the color that browsers and OSes should use if they customize the display of individual pages in their UIs with varying colors.
<meta name="theme-color" content="#ff69b4">
The content attribute extension can take any valid CSS color.
Currently, the theme-color meta extension is supported by Chrome 39+ for Android Lollipop and Firefox OS 2.1+.


https://github.com/h5bp/html5-boilerplate
