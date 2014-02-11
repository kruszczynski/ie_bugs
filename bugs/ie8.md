# IE 8 Bugs

### Your bug not here? Check out [common IE bugs](all.md)

#### Uploaded images weird mime types

In IE8, when you upload a `png` it has a unique to IE mime type `image/x-png`. This also happens for `jpeg` and `jpg`, they have a mime type `image/pjpeg`. One should be careful when validating attachment type.

#### CSS Selectors Limit

This is one of our favourites. IE8 (and IE 9) has various limits in CSS parsing:
* one CSS file can have up to 4096 selectors
* there can be up to 30 (or 31 depending on source) css files included in a page. No more!