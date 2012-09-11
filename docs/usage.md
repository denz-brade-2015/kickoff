Kickoff | [Documentation table of contents](README.md)

# Usage

Once you have cloned or downloaded Kickoff, creating a site or app
usually involves the following:

1. Set up the basic structure of the site.
2. Add some content, style, and functionality.
3. Run your site locally to see how it looks.
4. (Optionally run a build script to automate the optimization of your site -
   e.g. [ant build script](https://github.com/h5bp/ant-build-script) or [node
   build script](https://github.com/h5bp/node-build-script)).
5. Deploy your site.


## Basic structure

A basic Kickoff site initially looks something like this:

```
.
├── css
│   ├── kickoff.css
│   └── polyfills
│       └── box-sizing.htc
├── docs
├── img
│   └── ui
│       ├── glyphicons-halflings.png
│       └── glyphicons-halflings-white.png
├── js
│   ├── script.js
│   ├── plugins.js
│   ├── mobile-plugins.js
│   └── libs
│       ├── jquery.min.js
│       ├── modernizr.min.js
│       ├── zepto.min.js
│       ├── plugins
|           ├──
|           ├──
|           ├──
|           ├──
|           ├──
│           └──
│       └── polyfills
|           ├── jquery.easie.min.js
|           ├── jquery.imagesLoaded.min.js
|           ├── jquery.validation.min.js
|           ├── carouFredSel
|               ├── index.html
|               ├── jquery.carouFredSel.packed.js
|               └── jquery.carouFredSel.js
|           └── fancybox
|               ├── blank.gif
|               ├── fancybox_loading.gif
|               ├── fancybox_sprite.png
|               ├── jquery.fancybox.css
|               ├── jquery.fancybox.js
|               ├── jquery.fancybox.pack.js
|               └── helpers
|                   ├── fancybox_buttons.png
|                   ├── jquery.fancybox-buttons.css
|                   ├── jquery.fancybox-buttons.js
|                   ├── jquery.fancybox-thumbs.css
|                   └── jquery.fancybox-thumbs.js
├── less
│   ├── app.less
│   ├── button-groups.less
│   ├── buttons.less
│   ├── carousel.less
│   ├── choreographic-grid.less
│   ├── code.less
│   ├── forms.less
│   ├── grid-static.less
│   ├── kickoff.less
│   ├── layouts.less
│   ├── mixins.less
│   ├── normalize.less
│   ├── print.less
│   ├── responsive-utilities.less
│   ├── sprites.less
│   ├── tables.less
│   ├── typography.less
│   ├── utilities.less
│   ├── variables.less
│   └── wells.less
├── .htaccess
├── 404.html
├── index.html
├── humans.txt
├── robots.txt
├── crossdomain.xml
├── favicon.ico
└── [apple-touch-icons]
```

What follows is a general overview of each major part and how to use them.

### css

This directory should contain all your project's CSS files. It includes some
initial CSS to help get you started from a solid foundation. [About the
CSS](css.md).

### docs

This directory contains all the Kickoff documentation. You can use it
as the location and basis for your own project's documentation.

### js

This directory should contain all your project's JS files. Libraries, plugins,
and custom code can all be included here. It includes some initial JS to help
get you started. [About the JavaScript](js.md).

### .htaccess

The default web server config is for Apache. [About the .htaccess](htaccess.md).

Host your site on a server other than Apache? You're likely to find the
corresponding configuration file in our [server configs
repo](https://github.com/h5bp/server-configs). If you cannot find a
configuration file for your setup, please consider contributing one so that
others can benefit too.

### index.html

This is the default HTML skeleton that should form the basis of all pages on
your site. If you are using a server-side templating framework, then you will
need to integrate this starting HTML with your setup.

Make sure that you update the URLs for the referenced CSS and JavaScript if you
modify the directory structure at all.

If you are using Google Analytics, make sure that you edit the corresponding
snippet at the bottom to include your analytics ID.

### humans.txt

Edit this file to include the team that worked on your site/app, and the
technology powering it.

### robots.txt

Edit this file to include any pages you need hidden from search engines.

### crossdomain.xml

A template for working with cross-domain requests. [About
crossdomain.xml](crossdomain.md).

### icons

Replace the default `favicon.ico` and apple touch icons with your own. You
might want to check out Hans Christian's handy [Kickoff Favicon and
Apple Touch Icon
PSD-Template](http://drublic.de/blog/html5-boilerplate-favicons-psd-template/).