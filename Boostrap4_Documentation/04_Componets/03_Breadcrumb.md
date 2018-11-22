

Breadcrumb
Indicate the current page’s location within a navigational hierarchy that automatically adds separators via CSS.

Join over 300,000 developers using CircleCI's integration with GitHub.
ads via Carbon
Overview
Separators are automatically added in CSS through ::before and content.

Home
Home
Library
Home
Library
Data
Copy
<nav aria-label="breadcrumb">
  <ol class="breadcrumb">
    <li class="breadcrumb-item active" aria-current="page">Home</li>
  </ol>
</nav>

<nav aria-label="breadcrumb">
  <ol class="breadcrumb">
    <li class="breadcrumb-item"><a href="#">Home</a></li>
    <li class="breadcrumb-item active" aria-current="page">Library</li>
  </ol>
</nav>

<nav aria-label="breadcrumb">
  <ol class="breadcrumb">
    <li class="breadcrumb-item"><a href="#">Home</a></li>
    <li class="breadcrumb-item"><a href="#">Library</a></li>
    <li class="breadcrumb-item active" aria-current="page">Data</li>
  </ol>
</nav>
Accessibility
Since breadcrumbs provide a navigation, it’s a good idea to add a meaningful label such as aria-label="breadcrumb" to describe the type of navigation provided in the <nav> element, as well as applying an aria-current="page" to the last item of the set to indicate that it represents the current page.

For more information, see the WAI-ARIA Authoring Practices for the breadcrumb pattern.