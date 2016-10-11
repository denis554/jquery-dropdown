# jQuery Dropdown

Simple jquery dropdown

## Instalation

Download the latest version from GitHub

Include the CSS file in the head section:

```html
<link rel="stylesheet" href="jquery.dropdown.css">
```

Include the JS file before the `&lt;/body&gt;`:

```html
<script src="jquery.dropdown.js"></script>
```

Add initialization

```js
$(document).ready(function() {
	$('[data-dropdown-role="dropdown"]').dropdown();
});
```

And now create the dropdown html like in demo

```html
<div data-dropdown-role="dropdown" class="dropdown">
	<button data-dropdown-role="trigger" class="dropdown__trigger">Dropdown<span class="dropdown__caret"></span></button>
	<div data-dropdown-role="drop-menu" class="dropdown__menu">
		<ul>
			<li tabindex="0" class="dropdown__item">Item 1</li>
			<li tabindex="0" class="dropdown__item">Item 2</li>
			<li tabindex="0" class="dropdown__item">Item 3</li>
			<li tabindex="0" class="dropdown__item">Item 4</li>
			<li tabindex="0" class="dropdown__item">Item 5</li>
			<li tabindex="0" class="dropdown__item">Item 6</li>
			<li tabindex="0" class="dropdown__item">Item 7</li>
			<li tabindex="0" class="dropdown__item">Item 8</li>
		</ul>
	</div>
</div>
```

if you want use custom html, mark parts of your dropdown using data attributes

* `data-dropdown-role="trigger"`
* `data-dropdown-role="drop-menu"`

## Options

### base
* Type: *String*
* Default: *dropdown*

Base class name.

### open
* Type: *String*
* Default: *dropdown_open*

Open class name. Add on open dropdown.

### disabled
* Type: *String*
* Default: *dropdown_disabled*

Disabled class name.


## Events

Firs get jquery object of your dropdown

```js
var $dropdown = $('[data-dropdown-role="dropdown"]');
```

### opened.dropdown

Trigger when dropdown is opened.

```js
$('[data-dropdown-role="dropdown"]').on('opened.dropdown', function(event) {
	event.preventDefault();
	console.log(event.target, 'opened');
});
```

### closed.dropdown

Trigger when dropdown is closed.

```js
$('[data-dropdown-role="dropdown"]').on('closed.dropdown', function(event) {
	event.preventDefault();
	console.log(event.target, 'closed');
});
```



## License
[The MIT License (MIT)](LICENSE)
