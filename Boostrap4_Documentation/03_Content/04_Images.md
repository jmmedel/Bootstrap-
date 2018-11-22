

Images
Documentation and examples for opting images into responsive behavior (so they never become larger than their parent elements) and add lightweight styles to them—all via classes.

All the tools your team needs in one place. Slack: Where work happens.
ads via Carbon
Responsive images
Images in Bootstrap are made responsive with .img-fluid. max-width: 100%; and height: auto; are applied to the image so that it scales with the parent element.

100%x250Copy
<img src="..." class="img-fluid" alt="Responsive image">
SVG images and IE 10
In Internet Explorer 10, SVG images with .img-fluid are disproportionately sized. To fix this, add width: 100% \9; where necessary. This fix improperly sizes other image formats, so Bootstrap doesn’t apply it automatically.

Image thumbnails
In addition to our border-radius utilities, you can use .img-thumbnail to give an image a rounded 1px border appearance.

200x200
Copy
<img src="..." alt="..." class="img-thumbnail">
Aligning images
Align images with the helper float classes or text alignment classes. block-level images can be centered using the .mx-auto margin utility class.

200x200200x200Copy
<img src="..." class="rounded float-left" alt="...">
<img src="..." class="rounded float-right" alt="...">
200x200Copy
<img src="..." class="rounded mx-auto d-block" alt="...">
200x200
Copy
<div class="text-center">
  <img src="..." class="rounded" alt="...">
</div>
Picture
If you are using the <picture> element to specify multiple <source> elements for a specific <img>, make sure to add the .img-* classes to the <img> and not to the <picture> tag.

Copy
​<picture>
  <source srcset="..." type="image/svg+xml">
  <img src="..." class="img-fluid img-thumbnail" alt="...">
</picture>
