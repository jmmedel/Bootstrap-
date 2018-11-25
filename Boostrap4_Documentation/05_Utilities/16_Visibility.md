

Visibility
Control the visibility, without modifying the display, of elements with visibility utilities.

The new generation of project management tools is here and it’s visual.
ads via Carbon
Set the visibility of elements with our visibility utilities. These do not modify the display value at all and are helpful for hiding content from most users, but still keeping them for screen readers.

Apply .visible or .invisible as needed.

<div class="visible">...</div>
<div class="invisible">...</div>
// Class
.visible {
  visibility: visible;
}
.invisible {
  visibility: hidden;
}

// Usage as a mixin
.element {
  @include invisible(visible);
}
.element {
  @include invisible(hidden);
}
