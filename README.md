# Global Cursor

Apply the CSS cursor property to the high z-index element so that during a specific action, the cursor remains fixed to the desired style.

## Usage

```ts
import { cursor } from "global-cursor";

knob.addEventListener("pointerdown", (ev) => {
  ev.preventDefault();
  cursor.show("grabbing");
});

knob.addEventListener("pointerup", (ev) => {
  cursor.hide();
});
```

## Methods

### `cursor.show(cursorType: CursorType)`

`cursorType` is a value permitted for the CSS cursor property: [CSS cursor Property](https://www.w3schools.com/cssref/pr_class_cursor.php)

### `cursor.hide()`

Hide the cursor.

### `cursor.setZIndex(value: number)`

Change the z-index property of the element to which the cursor is applied. default value: 99999999
