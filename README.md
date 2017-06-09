HTML and CSS Template
=====================

Version 1.2, March 10, 2017

This is template for web page. Includes:

- valid HTML document with all necessary tags in the head section;
- CSS basis for easy start;
- humans.txt example file;
- robots.txt example file;
- sitemap.xml example file;
- set of favicons of basic necessary resolutions;

Used Components:

- [Normalize.css 5.0.0](http://necolas.github.io/normalize.css/);
- [Bootstrap 3.3.7](http://getbootstrap.com/) as basis of all styles;

Browsers support: Chrome, Firefox, Opera, IE 8+, Safari 6+.

Recomend to minimize and compile css styles to use on production.


HEAD section specias
--------------------

### Mobile optimized page

Tag `meta` with name="viewport" and css rule '@-ms-viewport'
in 'assets/basis.css' tells browser that the page is mobile optimized.
There are two old tags for the same task, I removed from html document.
They used by Palm devices and Windows Mobile devices:

    <meta name="HandheldFriendly" content="True">
    <meta name="MobileOptimized" content="320">

### Old IE compatibility

With tag `<meta http-equiv="x-ua-compatible" content="IE=edge,chrome=1">`
IE uses the highest supported
[document mode](https://msdn.microsoft.com/en-us/library/jj676915.aspx)
(actual for IE8-10).

[Html5shiv](https://github.com/aFarkas/html5shiv) adds HTML5 elements support
to IE 6-8

Tag `<meta http-equiv="msthemecompatible" content="no">` prevent to adjust
the OS theme to your website in IE. But this only for IE6 and Windows XP. Skip.

### Basic Page Info

Tags `title` and `meta` with name="description" gives basic information about
the page to search engines. They are required. Tag `meta` with name="keywords"
is optional and possibly ignored by search engines crawlers.

### Twitter card

With [Twitter Cards](https://dev.twitter.com/cards), you can attach rich photos,
videos and media experiences to Tweets, helping to drive traffic to your
website. Simply add a few lines of markup to your webpage, and users who Tweet
links to your content will have a “Card” added to the Tweet that’s visible
to their followers.

Tag `<meta name="twitter:card" content="summary">` enable Twitter card.
Title, description and image Twitter
[will get](https://dev.twitter.com/cards/getting-started#twitter-cards-and-open-graph)
from Open Graph tags.

Use other Twitter Card meta-tags only for
[special cases](https://dev.twitter.com/cards/types).

### Open Graph protocol

[The Open Graph protocol](http://ogp.me/) enables any web page to become
a rich object in a social graph. For instance, this is used on Facebook
to allow any web page to have the same functionality as any other object
[on Facebook](https://developers.facebook.com/docs/sharing/webmasters).

### Favicon

Build a correct favicon.ico file with ImageMagick:

    convert fav16.png fav32.png fav48.png favicon.ico

Or with [online service](http://icoconvert.com/).

### Apple touch icons

In tag `link` with rel="apple-touch-icon" you can set the Apple touch icon
[for Web Clip](https://developer.apple.com/library/content/documentation/AppleApplications/Reference/SafariWebContent/ConfiguringWebApplications/ConfiguringWebApplications.html).
Use this [guidelines](https://developer.apple.com/ios/human-interface-guidelines/graphics/app-icon/#app-icon-sizes).

### Microsoft application

With meta tags you can customize data of pinned site
[on Windows desktop](https://msdn.microsoft.com/en-us/library/dn255024.aspx)
and [for IE](https://msdn.microsoft.com/en-us/library/hh772707.aspx). Example:

    <meta name="application-name" content="HTML and CSS Template">
    <meta name="msapplication-tooltip" content="HTML and CSS Template by Dymio">
    <meta name="msapplication-starturl" content="http://github.com/dymio/html-css-template">
    <meta name="msapplication-TileColor" content=" #009900" />
    <meta name="msapplication-TileImage" content="ico/squareicon.png">
    <meta name="msapplication-square70x70logo" content="ico/smalltile.png" />
    <meta name="msapplication-square150x150logo" content="ico/mediumtile.png" />
    <meta name="msapplication-wide310x150logo" content="ico/widetile.png" />
    <meta name="msapplication-square310x310logo" content="ico/largetile.png" />

In the html document I use only top tags for Metro UI: TileColor and TileImage.


License
-------

[The MIT License (MIT)](https://opensource.org/licenses/MIT),
Copyright 2014 Ivan Dymkov.


Contributing
------------

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

Feel free to use code of the project as you want,
[create issues](https://github.com/dymio/html-css-template/issues)
or make pull requests.
