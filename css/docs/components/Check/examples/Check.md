---
id: Checkbox
section: components
cssPrefix: pf-c-check
---## Examples

### Basic

```html
<div class="pf-c-check">
  <input class="pf-c-check__input" type="checkbox" id="check-basic" name="check-basic" />
  <label class="pf-c-check__label" for="check-basic">Check</label>
</div>
```

### Checked

```html
<div class="pf-c-check">
  <input class="pf-c-check__input" type="checkbox" id="check-checked" name="check-checked" checked />
  <label class="pf-c-check__label" for="check-checked">Check checked</label>
</div>
```

### Label wrapping input

```html
<label class="pf-c-check" for="check-label-wrapping-input">
  <input class="pf-c-check__input" type="checkbox" id="check-label-wrapping-input" name="check-label-wrapping-input" />
  <span class="pf-c-check__label">Check label wraps input</span>
</label>
```

### Reversed

```html
<div class="pf-c-check">
  <label class="pf-c-check__label" for="check-reversed">Check reversed</label>
  <input class="pf-c-check__input" type="checkbox" id="check-reversed" name="check-reversed" /></div>
```

### Disabled

```html
<div class="pf-c-check">
  <input class="pf-c-check__input" type="checkbox" id="check-disabled" name="check-disabled" disabled />
  <label class="pf-c-check__label pf-m-disabled" for="check-disabled">Check disabled</label>
</div>
<div class="pf-c-check">
  <input class="pf-c-check__input" type="checkbox" id="check-disabled-2" name="check-disabled-2" checked disabled />
  <label class="pf-c-check__label pf-m-disabled" for="check-disabled-2">Check disabled checked</label>
</div>
```

### With description

```html
<div class="pf-c-check">
  <input class="pf-c-check__input" type="checkbox" id="check-with-description" name="check-with-description" />
  <label class="pf-c-check__label" for="check-with-description">Check with description</label>
  <div class="pf-c-check__description">Single-tenant cloud service hosted and managed by Red Hat that offers high-availability enterprise-grade clusters in a virtual private cloud on AWS od GCP.</div>
</div>
```

## Documentation

### Overview

The Check component is provided for use cases outside of forms. If it is used without label text ensure some sort of label for assistive technologies. (for example: `aria-label`)

If you extend this component or modify the styles of this component, then make sure any hover styles defined are applied to the clickable elements, like `<input>` or `<label>` since hover styles are used to convey the clickable target area of an element. To maximize the target area, use the example html where the `<label>` is the wrapping element.

### Accessibility

| Attribute  | Applied to                | Outcome                                                                                                           |
| ---------- | ------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| `disabled` | `<input type="checkbox">` | Indicates that the element is unavailable and removes it from keyboard focus. **Required when input is disabled** |

### Usage

| Class                      | Applied to                | Outcome                                                                    |
| -------------------------- | ------------------------- | -------------------------------------------------------------------------- |
| `.pf-c-check`              | `<div>`, `<label>`        | Initiates the check component. **Required**                                |
| `.pf-c-check__input`       | `<input type="checkbox">` | Initiates a check input. **Required**                                      |
| `.pf-c-check__label`       | `<label>`, `<span>`       | Initiates a label. **Required**                                            |
| `.pf-c-check__description` | `<div>`                   | Initiates a check description.                                             |
| `.pf-m-disabled`           | `.pf-c-check__label`      | Initiates a disabled style for labels. **Required when input is disabled** |
