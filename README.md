# nav-icons

These are the icons used by the image-based navigation bar.

## Stored on the CDN

The icons are published to the Brightspace CDN here:

> https://s.brightspace.com/lib/nav-icons/1.1.0/icon-name.svg

Do not reference the icons from GitHub, use the CDN location.

## Udpating Icons

If you need update, add or remove an icon, submit a pull request. Once approved and merged, the changes will need to be manually re-published to the CDN in a new version directory, and the LMS will need to be manually updated to reference the new version.

The SVG files should be properly formatted. This ensures that they will render at the correct size and in the correct color across all browsers. Follow these rules:
- native icon sizes need to be _exactly_ 60 x 60
- the `<svg>` element must:
  - have a `width` and `height` attribute which matches the size
  - not have an `id` or `data-name` attribute
- the `<svg>`'s `viewBox` attribute must:
  - have an origin beginning at `0 0`
  - be exactly square (e.g. `0 0 60 60`)
  - not contain negative values
- there should be no `<title>` element
- there should be no inline `<style>` are CSS classes -- all style for line fills should be applied directly to the SVG elements

The best way to have most of these rules applied for you automatically is to put the icon through [SVGOMG](https://jakearchibald.github.io/svgomg/) with the "remove title" and "prettify code" options selected.

Here's a sample of a properly formatted SVG:

```svg
<svg width="60" height="60" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 60 60">
    ...
</svg>
```
