

Screenreaders
Use screenreader utilities to hide elements on all devices except screen readers.

Startup checking built for the valley. Grow your business with 0.75% APY.
ads via Carbon
Hide an element to all devices except screen readers with .sr-only. Combine .sr-only with .sr-only-focusable to show the element again when it’s focused (e.g. by a keyboard-only user). Can also be used as mixins.

Copy
<a class="sr-only sr-only-focusable" href="#content">Skip to main content</a>
Copy
// Usage as a mixin
.skip-navigation {
  @include sr-only;
  @include sr-only-focusable;
}
