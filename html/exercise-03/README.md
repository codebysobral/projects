# Why use `rel="noopener noreferrer"`?

When using `target="_blank"`, the link opens in a new tab. Adding `rel="noopener noreferrer"` helps make this safer and more private.

* `noopener` prevents the new page from accessing the original page.
* `noreferrer` hides information about where the visitor came from.

For external links, using both is a simple security best practice.

```html id="e2h9s4"
<a
  href="https://example.com"
  target="_blank"
  rel="noopener noreferrer"
>
  Visit Website
</a>
```
