

Clearfix
Quickly and easily clear floated content within a container by adding a clearfix utility.

It's teamwork, but simpler, more pleasant and more productive.
ads via Carbon
Easily clear floats by adding .clearfix to the parent element. Can also be used as a mixin.

Copy
<div class="clearfix">...</div>
Copy
// Mixin itself
@mixin clearfix() {
  &::after {
    display: block;
    content: "";
    clear: both;
  }
}

// Usage as a mixin
.element {
  @include clearfix;
}
The following example shows how the clearfix can be used. Without the clearfix the wrapping div would not span around the buttons which would cause a broken layout.

Copy
<div class="bg-info clearfix">
  <button type="button" class="btn btn-secondary float-left">Example Button floated left</button>
  <button type="button" class="btn btn-secondary float-right">Example Button floated right</button>
</div>
