# All IE versions Bugs

#### input[type="file"] javascript manipulation

In IE, when you try to manipulate `input[type="file"]`, to create a custom image upload button for example (`$('button').click(function(){$('input[type="file"]).click()` is sufficient), IE will prevent the form from submitting returning `Access Denied` error.

