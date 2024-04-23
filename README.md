# Open Styled Templates
## Customizable Web Components
```html
<template id="custom-button-template">
  <style>
    button {
      padding: var(--button-padding, 8px 16px);
      border-radius: var(--button-border-radius, 4px);
      cursor: pointer;
    }

    /* Variants */
    button.primary {
      background-color: var(--button-primary-bg-color, #007bff);
      color: var(--button-text-color, white);
    }

    button.secondary {
      background-color: var(--button-secondary-bg-color, #6c757d);
      color: var(--button-text-color, white);
    }

    button.disabled {
      background-color: var(--button-disabled-bg-color, #f8f9fa);
      color: var(--button-disabled-text-color, #6c757d);
      cursor: not-allowed;
    }
  </style>
  <button id="button">
    <slot></slot> <!-- with or without slot -->
  </button>
</template>
```
### Custom Root Properties
```css
:root {
  --button-padding: 8px 16px;
  --button-border-radius: 4px;
  --button-primary-bg-color: #007bff;
  --button-secondary-bg-color: #6c757d;
  --button-text-color: white;
  --button-disabled-bg-color: #f8f9fa;
  --button-disabled-text-color: #6c757d;
}
```

