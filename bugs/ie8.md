# IE 8 Bugs

### Your bug not here? Check out [common IE bugs](all.md)

#### Uploaded images weird mime types

In IE8, when you upload a `png` it has a unique to IE mime type `image/x-png`. This also happens for `jpeg` and `jpg`, they have a mime type `image/pjpeg`. One should be careful when validating attachment type.

#### CSS Selectors Limit

This is one of our favourites. IE8 (and IE 9) has various limits in CSS parsing:
* one CSS file can have up to 4096 selectors
* there can be up to 30 (or 31 depending on who you ask) css files included in a page. No more!

#### `console.*` problem

In IE 8, when a js file calls a `console` object, the script will break unless developer tools are open. This is most commonly caused by calling `console.log("this is foo: " + foo);`

#### JSON objects comma issue

In IE 8, when an object is defined with a trailing `,` for convenience for example
```javascript
{
	mambo: 'number five',
	livin: 'la vida loca',
	eye: 'of the tiger',
}
```
the json will not be parsed correctly. This is the reason why many libraries create object in a following manner:
```javascript
{
	tony: 'hawk'
	, mr: 'T'
	, a: 'team'
}
```

#### `:checked` CSS selector not working

In IE8 the `:checked` CSS selector does not work in IE8. But `[checked='checked']` attribute selector does work. This however will not work in modern browsers.
