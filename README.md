# html-nav
The navlinks data structure is an array of a denormalized navbar entries; each entry contains an object:
  - campus: Which catalog ("university", "providence", "other", etc)
  - section: The parent of the current item
  - name: The display name
  - url: The link target; this is the section of all child links

Goal is to create a function that will be called with a specific campus and a specific path and will return a *string* that contains properly formed XHTML for the navbar: a set of nested unordered lists that can be used in the navbar on the left to show the user "where" they are in the site.

This small project leverages: jQuery, some polyfills on bind and filter() for legacy browsers, plus home-grown JavaScript.
