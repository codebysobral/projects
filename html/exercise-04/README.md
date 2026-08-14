# When to Use `alt` on Images

Use the `alt` attribute to provide text alternatives for images.

## Use `alt=""`

Use an empty `alt` when the image is **decorative** and does not add meaningful information.

```html
<img src="divider.png" alt="">
```

This tells screen readers to ignore the image.

## Use a Descriptive `alt`

Use descriptive text when the image **communicates information** or has a purpose.

```html
<img src="team.jpg" alt="Our development team standing in front of the office">
```

The description should be concise and explain the image's meaning, not every visual detail.

## Quick Rule

* **Decorative image** → `alt=""`
* **Informative or functional image** → descriptive `alt`
* **Never omit `alt`** on meaningful images
