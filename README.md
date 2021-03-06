# Specify Image Dimensions 

Automatically specify image dimensions that are missing width and/or height attributes. Helps with website speed tools.

## Description 
A simple and lightweight plugin that scans your website and automatically sets the appropriate image dimensions that are missing a `width` and/or `height` attributes in your `<img>` tags.

For example, here are some images with no dimensions set:

`
<img src="http://link.to/some/img1.jpg" id="123" alt="Some Alt" />
<img class="some-class" src="http://link.to/some/img2.jpg" alt="Another Alt" />
<img class="another-class" src="http://link.to/some/img2.jpg" width="500" />
`

The plugin will get the actual image dimension and insert the width and height:

`
<img src="http://link.to/some/img1.jpg" alt="Some Alt" id="123" width="500" height="350" />
<img src="http://link.to/some/img1.jpg" alt="Another Alt" class="some-class" width="500" height="350" />
<img src="http://link.to/some/img1.jpg" class="another-class" width="500" height="350" />
`

### Why is this important? 
Specifying a `width` and `height` for all images allows for faster rendering by eliminating the need for unnecessary re-flows and repaints. This is particularly helpful with website speed tools such as <a href="https://gtmetrix.com">GTmetrix</a> and <a href="https://developers.google.com/speed/pagespeed/">Google's PageSpeed</a>.

> **More details from Google**
>
> When the browser lays out the page, it needs to be able to flow around replaceable elements such as images. It can begin to render a page even before images are downloaded, provided that it knows the dimensions to wrap non-replaceable elements around. If no dimensions are specified in the containing document, or if the dimensions specified don't match those of the actual images, the browser will require a reflow and repaint once the images are downloaded. To prevent reflows, specify the width and height of all images, either in the HTML <img> tag, or in CSS.
>
> **Reference**: [GTmetrix](https://gtmetrix.com/specify-image-dimensions.html)

## Frequently Asked Questions 

### How does it work? 
The plugin will scan the contents in 

### Why is this important? 
Specifying a `width` and `height` for all images allows for faster rendering by eliminating the need for unnecessary re-flows and repaints. This is particularly helpful with website speed tools such as <a href="https://gtmetrix.com">GTmetrix</a> and <a href="https://developers.google.com/speed/pagespeed/">Google's PageSpeed</a>. More information can be found [here](https://developers.google.com/speed/pagespeed/module/filter-image-optimize#resize-image-dimensions).

### I'd like to contribute to this plugin and help improve it 
That's easy! If you have a GitHub account, you're more than welcome to share your contribution to our plugin which can be found [here](https://github.com/factmaven/specify-image-dimensions).

## Changelog 

### 1.0.0 08/21/16 
* Initial release, huzzah!