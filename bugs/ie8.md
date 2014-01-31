# IE 8 Bugs

#### image mime types

In IE8, when you upload a `png` it has a unique to IE mime type `image/x-png`. This also happens for `jpeg` and `jpg`, they have a mime type `image/pjpeg`. One should be careful when validating attachment type.