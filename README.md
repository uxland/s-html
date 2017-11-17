# &lt;s-html&gt;

Element wrapper of `.innerHTML` for data binding with HTML elements.

## Usage

### Example 1

Localize text with HTML elements using [app-localize-behavior](https://github.com/PolymerElements/app-localize-behavior).

locales.json
```json
{
"text": "<span>Settings</a>"
}
```

HTML
```html
<s-html html="[[localize('text')]]"></s-html>
```

### Example 2

Using element content styled with CSS.

locales.json
```json
{
"text": "<span class=\"red\">Settings</span>"
}
```

CSS
```css
.red {
  color: red;
}
```

HTML
```html
<s-html html="[[localize('text')]]"></s-html>
```

### Example 3

Using element content styled with CSS within an element.

locales.json
```json
{
"text": "<span class=\"red\">Settings</span>"
}
```

CSS
```css
.red {
  color: red;
}
```

HTML
```html
<s-html html="[[localize('text')]]"><custom-element></custom-element></s-html>
```

### Example 4

Unescape escaped HTML elements.

locales.json
```json
{
"text": "polymer &lt;br&gt;"
}
```

HTML
```html
<s-html unescape html="[[localize('text')]]"></s-html>
```

## Installation

`bower i uxland/s-html -S`

## License

Apache 2.0
