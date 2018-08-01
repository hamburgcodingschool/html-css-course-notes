# HTML

## Intro

HTML is a markup language. That means it is used to give a document a semantic structure and annotates the content of the document.

A HTML document consists entirely of HTML elements. These elements are described by **tags**. **tags** are surrounded by angle brackets (`<` and `>`).

In HTML, basically all elements are predefined. Which means you can't just make up some. Browsers handle made up elements very generously, but the specification defines a fixed set of elements. All those elements have a special purpose. Some are very specific and others have a wide range of use cases.

HTML elements can add content directly to the web page like so by using self closing **tags**:

```html
<tag attribute1="value1" attribute2="value2" />
```

`<img />` and `<input />` are examples for such elements. These elements have no closing **tag** part.

Other elements use **tags** to surround and annotate the content that should be shown. These elements can contain other **tags** as well. They can be nested indefinitely.

```html
<tag attribute1="value1" attribute2="value2">content</tag>
```

Examples for surrounding elements are `<p>content</p>` or `<div>content</div>`. These elements have an opening and a closing **tag**.

The **tags** itself (with all the attributes) will never be show to the user but will instruct the browser on how to show the content.

## Usage

### Tags

```html
<html>

    <head> <!-- a head tag (start-tag) -->
        <title>Page Title</title>
    </head> <!-- a head tag (end-tag) -->

    <body>
    …
    </body>

</html>
```

Here we see some elements togethe rin a way that marks out a standard web page.

The `<html>` element has two other elements as children. The `<head>` and the `<body>`. These two elements can have other elements as content (called children). In this example the `<body>` is empty but the `<head>` has the `<title>` element as child and could have several others.

Next we look only at the body element. This is the element that normally has the most children and caries the content of the whole page.

```html
<body>
    <p>
        Even the worst thing we can do here is good. You can create the world you want to see and be a part of. <a href="http://you.com">You</a> have that power. Just make a decision and let it go. As trees get older they lose their chlorophyll.
    </p>

    <img src="path/to/image.png" /> <!-- a non closing element -->
</body>
```

The HTML boilerplate is removed to focus on the `<body>`. The `<body>` now includes several elements. An `<p>`, `<a>` and an `<img>` element.

The **paragraph** element (`<p>`) normally holds just texts but can also include other elements. It does not make sense for all elements to sit inside a paragraph. Common children of a paragraph are `<img>`, `<a>` and `<span>`.

The same is true for the **anchor** (`<a>`) which specifies a link to another document. Anchor elements describe the things that you can click on in a browser and suddenly end up on a completely different page. These are the **hyperlinks**. As for the **paragraph** some elements make sense to put inside other then text. Like an `<img>` element. But it makes no sense to put another anchor inside an anchor. Although it might not be against the specification.

Lastly in our example we have an **image** element (`<img>`). This is a typical non-closing element. The image element itself defines the content. It is not possible to add anything _inside_ an image.

### Attributes

In the example from before we had the **anchor** and **image** elements. One was a closing and one was a non-closing element. But both had attributes in the opening tag.

```html
<a href="http://you.com">You</a>

<img src="path/to/image.png" />
```

Attributes are special properties of an element that can be defined in the opening tag. An anchor element does need some information of where the other webpage is located. An image needs the file that should be shown as image.

There are lots and lots of different attributes for elements. They are not the same for each element. Some of the attributes are only available for certain elements. The anchor element is the only one that has an `href` (hypertext reference) attribute because only the anchor elements need to handle this hypertext reference to show tell the browser the new web page.

The `src` (source) attribute of the image, on the other hand, is used in many different elements because other elements need to handle some kind of source for their purpose.

The attribute that is probably the most common across all elements is the `class` attribute. The `class` attribute is used as an interface between HTML and the other two big web languages, JavaScript and CSS. JavaScript and CSS using the `class` attribute to select specific elements and add functionality or enhance presentation of that element.
