---
id: Switch
section: components
cssPrefix: pf-c-switch
---## Examples

### Basic

```html
<label class="pf-c-switch" for="switch-with-label-1">
  <input class="pf-c-switch__input" type="checkbox" id="switch-with-label-1" aria-labelledby="switch-with-label-1-on" name="switchExample1" checked />
  <span class="pf-c-switch__toggle"></span>
  <span class="pf-c-switch__label pf-m-on" id="switch-with-label-1-on" aria-hidden="true">Message when on</span>
  <span class="pf-c-switch__label pf-m-off" id="switch-with-label-1-off" aria-hidden="true">Message when off</span>
</label>
<br/>
<br/>
<label class="pf-c-switch" for="switch-with-label-2">
  <input class="pf-c-switch__input" type="checkbox" id="switch-with-label-2" aria-labelledby="switch-with-label-2-on" name="switchExample2" />
  <span class="pf-c-switch__toggle"></span>
  <span class="pf-c-switch__label pf-m-on" id="switch-with-label-2-on" aria-hidden="true">Message when on</span>
  <span class="pf-c-switch__label pf-m-off" id="switch-with-label-2-off" aria-hidden="true">Message when off</span>
</label>
```

### Without label

```html
<label class="pf-c-switch" for="switch-with-icon-1">
  <input class="pf-c-switch__input" type="checkbox" id="switch-with-icon-1" aria-label="switch is off" name="switchExample3" checked />
  <span class="pf-c-switch__toggle">
    <span class="pf-c-switch__toggle-icon">
      <i class="fas fa-check" aria-hidden="true"></i>
    </span>
  </span>
</label>
<br/>
<br/>
<label class="pf-c-switch" for="switch-with-icon-2">
  <input class="pf-c-switch__input" type="checkbox" id="switch-with-icon-2" aria-label="switch is off" name="switchExample4" />
  <span class="pf-c-switch__toggle">
    <span class="pf-c-switch__toggle-icon">
      <i class="fas fa-check" aria-hidden="true"></i>
    </span>
  </span>
</label>
```

### Disabled

```html
<label class="pf-c-switch" for="switch-disabled-1">
  <input class="pf-c-switch__input" type="checkbox" id="switch-disabled-1" aria-labelledby="switch-disabled-1-on" name="switchExample5" disabled checked />
  <span class="pf-c-switch__toggle"></span>
  <span class="pf-c-switch__label pf-m-on" id="switch-disabled-1-on" aria-hidden="true">Message when on</span>
  <span class="pf-c-switch__label pf-m-off" id="switch-disabled-1-off" aria-hidden="true">Message when off</span>
</label>
<br/>
<br/>
<label class="pf-c-switch" for="switch-disabled-2">
  <input class="pf-c-switch__input" type="checkbox" id="switch-disabled-2" aria-labelledby="switch-disabled-2-on" name="switchExample6" disabled />
  <span class="pf-c-switch__toggle"></span>
  <span class="pf-c-switch__label pf-m-on" id="switch-disabled-2-on" aria-hidden="true">Message when on</span>
  <span class="pf-c-switch__label pf-m-off" id="switch-disabled-2-off" aria-hidden="true">Message when off</span>
</label>
```

## Documentation

### Overview

A switch is an alternative to the checkbox component.

Use a switch when your user needs to perform instantaneous actions without confirmation.

Use checkbox if your user has to perform additional steps for changes to become effective.

### Accessibility

| Attribute                                     | Applied to                | Outcome                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| --------------------------------------------- | ------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `aria-labelledby="..."` or `aria-label="..."` | `.pf-c-switch__input`     | Indicates the action triggered by the switch. If an additional text label is included with the switch besides `.pf-c-switch__label.pf-m-on`, then `aria-labelledby` can reference the `id` of this text, or this text can be used as the value for `aria-label`. If the text included for `.pf-c-switch__label.pf-m-on` provides additional meaning to the primary label that's referenced, then it can also be represented as part of the `aria-labelledby` or `aria-label` attribute. **Required** |
| `for`                                         | `<label>`                 | Each `<label>` must have a `for` attribute that matches its input id. **Required**                                                                                                                                                                                                                                                                                                                                                                                                                   |
| `id`                                          | `<input type="checkbox">` | Each `<input>` must have an `id` attribute that matches its label's `for` value. **Required**                                                                                                                                                                                                                                                                                                                                                                                                        |
| `id`                                          | `.pf-c-switch__label`     | Each `.pf-c-switch__label` must have an `id` attribute that matches the `aria-labelledby` on `.pf-c-switch__input`.                                                                                                                                                                                                                                                                                                                                                                                  |
| `checked`                                     | `.pf-c-switch__input`     | Indicates that the input is checked                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| `disabled`                                    | `.pf-c-switch__input`     | Indicates that the input is disabled                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| `aria-hidden="true"`                          | `.pf-c-switch__label`     | Hides the text from the screen reader.                                                                                                                                                                                                                                                                                                                                                                                                                                                               |

### Usage

| Class                       | Applied to                | Outcome                                                                                        |
| --------------------------- | ------------------------- | ---------------------------------------------------------------------------------------------- |
| `.pf-c-switch`              | `<label>`                 | Initiates a switch. **Required**                                                               |
| `.pf-c-switch__input`       | `<input type="checkbox">` | Hide the checkbox inside the switch. **Required**                                              |
| `.pf-c-switch__toggle`      | `<span>`                  | Initiates the toggle inside the switch. **Required**                                           |
| `.pf-c-switch__toggle-icon` | `<span>`                  | Initiates the switch toggle icon wrapper. **Required when the switch is used without a label** |
| `.pf-c-switch__label`       | `<span>`                  | Initiates a label inside the switch.                                                           |
| `.pf-m-on`                  | `.pf-c-switch__label`     | Modifies the switch label to display the on message.                                           |
| `.pf-m-off`                 | `.pf-c-switch__label`     | Modifies the switch label to display the off message.                                          |
