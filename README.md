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

## License
[The MIT License (MIT)](LICENSE)
