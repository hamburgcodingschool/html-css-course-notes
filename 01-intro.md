# What is a website

In general a website is a collection of documents that are suitable for displaying in web browser like Google Chrome, Mozilla Firefox, Microsoft Edge, Safari and others.

These documents (web pages) are simple text files usually written in HTML (Hypertext Markup Language).

An example of a very basic HTML file that would render in a browser.

```html
<html>
    <head>
    <title>Website Title</title>
    </head>

    <body>
        The website Content.
    </body>
</html>
```

The web pages can be linked together with special HTML to form a web site.

Browsers read the single web page and render them according to the markup. Browsers are also able to render media content like images, video and audio which are referenced in the markup of a page.

With the use additional languages like CSS and JavaScript the presentation can be enhanced and more functionality can be added.

Although the underlying technologies may vary, every website you visit with your browser is using a combination of HTML, CSS and Javascript to show you the content.

To see examples in the wild go to any website and find the menu entry for showing the sources. In Google Chrome use `View -> Developer -> View Source`.

Here are some examples of the source of well know webpages.

google.de

```html
<!doctype html>
<html itemscope="" itemtype="http://schema.org/WebPage" lang="en-DE">

<head>
   <meta content="/images/branding/googleg/1x/googleg_standard_color_128dp.png" itemprop="image">
   <link href="/images/branding/product/ico/googleg_lodp.ico" rel="shortcut icon">
   <meta content="origin" name="referrer">
   <title>Google</title>
</head>
<body>
…
```

twitter.com

```html
<!DOCTYPE html>
<html lang="de">

<head>
   <meta charset="utf-8" />
   <title>Twitter</title>
   <style>
       body {
           background-color: #ffffff;
           font-family: sans-serif;
       }
       …
```

wordpress.com

```html
<!DOCTYPE html>
<html lang="de" class="webp" dir="ltr">
<head>
	<meta charset="UTF-8">
	<meta http-equiv="x-ua-compatible" content="IE=Edge">
	<title>WordPress.com: Erstelle eine kostenlose Website oder einen kostenlosen Blog</title>
	<meta name="apple-mobile-web-app-title" content="WP.com">
	<meta name="google-site-verification" content="Q9OTgmFGvbuu-bnRYsyoA-MXgythlBvu6gZJry9XxMA" />


	</head>
    <body id="wpcom-home" class="hp-rey de">
    <header class="masterbar is-transparent">
```

They are very different in use of single elements but use essentially the same techniques as private blog would do.
