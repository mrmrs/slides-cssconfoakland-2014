# Slides from my talk at CSSCONF - Oakland 2014

I recently gave a talk at CSSCONF in Oakland. Here are my slides.

For those of you who attended - or to anyone who watches the video,
I'd like to clarify a few points.

At one point I kind of champion inline styles. I forgot to clarify I mean the mental model that
inline styles provide. Inline styles are actually quite slow to render to the browser
as each declaration has a one to one relationship with the dom. A single purpose class however
i.e ```.bg-red { background-color: red; }``` has a one to many relationship with the dom and is
faster for the browser to paint. I find this is the same type of encapsulation - but it's far
easier to maintain.

I don't know if I somehow missed it during my talk or if slide 25 just didn't load for some reason - but I'd
be remiss to not call attention to the one quote that completely changed my workflow when writing css.

In Nicole Sullivan's post 'The media object saves hundreds of lines of code' she has the following quote:

> When I’m building a new object, the first thing I do is to figure out which parts are reusable components, and define what I know and do not know about them.

This is not something I had ever thought of before.
When I am building components I now stop and write out notes about all the things I know and all the things I don't know.
I've found that being informed on what you don't know, will help you in keeping concerns separated - and that your abstractions are on point.
Bad css is full of assumptions. Understanding where you can't make assumptions can help you write code that works in more contexts.

## All of CSS in one file
If you want to see my experiment with putting the entire css language into one file it's called (css unabridged)[http://github.com/mrmrs/css-unabridged].
I've tried to make it as verbose as possible and it is currently 20.15kb minified and gzipped.

## Reading

These articles have helped change how I think about writing css,
html. Some of them are not actually articles about front-end development,
but still introduced concepts to me that changed how I approached authoring
code for users.

* [Material honesty on the web - Kevin Goladman](http://alistapart.com/article/material-honesty-on-the-web)
* [The media object saves hundreds of lines of code - Nicole Sullivan](http://www.stubbornella.org/content/2010/06/25/the-media-object-saves-hundreds-of-lines-of-code/)
* [About HTML semantics and front end architecture - Nicolas Gallagher](http://nicolasgallagher.com/about-html-semantics-front-end-architecture/)
* [A classless class - Harry Roberts](http://csswizardry.com/2012/10/a-classless-class-on-using-more-classes-in-your-html/)
* [I'm sick of your tiny tiny type - Brent Jackson](http://jxnblk.tumblr.com/post/41796724549/im-sick-of-your-tiny-tiny-type)
* [Code smells in CSS - Harry Roberts](http://csswizardry.com/2012/11/code-smells-in-css/)

This article is a little more technical - but gives some interesting insight into how chrome handles painting to the screen.
[GPU accelerated compositing in chrome](http://www.chromium.org/developers/design-documents/gpu-accelerated-compositing-in-chrome)

## License

The MIT License (MIT)

Copyright (c) 2014 @mrmrs

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
