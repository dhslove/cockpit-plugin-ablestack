---
id: Spinner
section: components
cssPrefix: pf-c-spinner
---## Examples

### Basic

```html
<span class="pf-c-spinner" role="progressbar" aria-valuetext="Loading...">
  <span class="pf-c-spinner__clipper"></span>
  <span class="pf-c-spinner__lead-ball"></span>
  <span class="pf-c-spinner__tail-ball"></span>
</span>
```

### Multiple sizes

```html
<span class="pf-c-spinner pf-m-sm" role="progressbar" aria-valuetext="Loading...">
  <span class="pf-c-spinner__clipper"></span>
  <span class="pf-c-spinner__lead-ball"></span>
  <span class="pf-c-spinner__tail-ball"></span>
</span>
<span class="pf-c-spinner pf-m-md" role="progressbar" aria-valuetext="Loading...">
  <span class="pf-c-spinner__clipper"></span>
  <span class="pf-c-spinner__lead-ball"></span>
  <span class="pf-c-spinner__tail-ball"></span>
</span>
<span class="pf-c-spinner pf-m-lg" role="progressbar" aria-valuetext="Loading...">
  <span class="pf-c-spinner__clipper"></span>
  <span class="pf-c-spinner__lead-ball"></span>
  <span class="pf-c-spinner__tail-ball"></span>
</span>
<span class="pf-c-spinner pf-m-xl" role="progressbar" aria-valuetext="Loading...">
  <span class="pf-c-spinner__clipper"></span>
  <span class="pf-c-spinner__lead-ball"></span>
  <span class="pf-c-spinner__tail-ball"></span>
</span>
```

<br />
<br />
<br />
## SVG spinner

### SVG spinner basic

```html
<svg class="pf-c-spinner" role="progressbar" aria-valuetext="Loading..." viewBox="0 0 100 100">
  <circle class="pf-c-spinner__path" cx="50" cy="50" r="45" fill="none"></circle>
</svg>
```

### SVG spinner, multiple sizes

```html
<svg class="pf-c-spinner pf-m-sm" role="progressbar" aria-valuetext="Loading..." viewBox="0 0 100 100">
  <circle class="pf-c-spinner__path" cx="50" cy="50" r="45" fill="none"></circle>
</svg>
<svg class="pf-c-spinner pf-m-md" role="progressbar" aria-valuetext="Loading..." viewBox="0 0 100 100">
  <circle class="pf-c-spinner__path" cx="50" cy="50" r="45" fill="none"></circle>
</svg>
<svg class="pf-c-spinner pf-m-lg" role="progressbar" aria-valuetext="Loading..." viewBox="0 0 100 100">
  <circle class="pf-c-spinner__path" cx="50" cy="50" r="45" fill="none"></circle>
</svg>
<svg class="pf-c-spinner pf-m-xl" role="progressbar" aria-valuetext="Loading..." viewBox="0 0 100 100">
  <circle class="pf-c-spinner__path" cx="50" cy="50" r="45" fill="none"></circle>
</svg>
```

### SVG spinner, custom size

```html
<svg class="pf-c-spinner" role="progressbar" aria-valuetext="Loading..." viewBox="0 0 100 100" style="--pf-c-spinner--diameter: 80px;">
  <circle class="pf-c-spinner__path" cx="50" cy="50" r="45" fill="none"></circle>
</svg>
```

## Documentation

### Accessibility

| Attribute                     | Applied to      | Outcome                                                                               |
| ----------------------------- | --------------- | ------------------------------------------------------------------------------------- |
| `role="progressbar"`          | `.pf-c-spinner` | Indicates to assistive technologies that this is an indeterminate progress indicator. |
| `aria-valuetext="Loading..."` | `.pf-c-spinner` | Describes content that is being loaded, while it is loading.                          |

Note: If the spinner is showing that loading of a particular region of a page is in process, the author should use `aria-describedby` to point to the status, and set the `aria-busy` attribute to `true` on the region until it is finished loading.

Note: A [live region](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/ARIA_Live_Regions) must be present before changing its status in order for the change to be read.

### Usage

| Class                      | Applied to | Outcome                                                                          |
| -------------------------- | ---------- | -------------------------------------------------------------------------------- |
| `.pf-c-spinner`            | `<span>`   | Creates a spinner component. The default is an extra large spinner. **Required** |
| `.pf-c-spinner__clipper`   | `<span>`   | Creates the spinning line. **Required**                                          |
| `.pf-c-spinner__lead-ball` | `<span>`   | Rounds out the beginning of the spinning line. **Required**                      |
| `.pf-c-spinner__tail-ball` | `<span>`   | Rounds out the end of the spinning line. **Required**                            |

### SVG variant

| Class                      | Applied to      | Outcome                                                                          |
| -------------------------- | --------------- | -------------------------------------------------------------------------------- |
| `.pf-c-spinner`            | `<svg>`         | Creates a spinner component. The default is an extra large spinner. **Required** |
| `.pf-c-spinner__path`      | `<circle>`      | Creates a spinner circle component. **Required**                                 |
| `--pf-c-spinner--diameter` | `.pf-c-spinner` | Modifies the value for `--pf-c-spinner--diameter` declaration.                   |

### Modifiers

| Class      | Applied to      | Outcome                         |
| ---------- | --------------- | ------------------------------- |
| `.pf-m-sm` | `.pf-c-spinner` | Creates a small spinner.        |
| `.pf-m-md` | `.pf-c-spinner` | Creates a medium spinner.       |
| `.pf-m-lg` | `.pf-c-spinner` | Creates a large spinner.        |
| `.pf-m-xl` | `.pf-c-spinner` | Creates an extra-large spinner. |
