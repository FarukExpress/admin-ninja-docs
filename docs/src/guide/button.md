# Button

Button is a component that can be used to trigger an action or event, such as submitting a form, opening a dialog, canceling an action, or performing a delete operation.

## Basic Buttons

```js
import Button from "@/components/Button";
const ButtonPage = () => {
  return (
    <div>
      <Button text="primary" className="btn-primary" />
    </div>
  );
};
```

::: tip
You can use `className` props for button type. Available types: `className="btn-primary"`, `className="btn-secondary"`, `className="btn-success"`, `className="btn-info"`, `className="btn-danger"`, `className="btn-warning"`,
:::

::: info Outline Buttons
You can use `className` props for for an outline button. For example: `className="btn-outline-primary"`, `className="btn-outline-secondary"`
:::

::: info Light Color Buttons
Just add an extra class `light` to the className for a light color button. For example: `className="btn-primary light"`, `type="btn-secondary light"`
:::

::: info Raised Buttons
Just add an extra class `shadow-base2` to the className for a raised button. For example: `className="btn-primary shadow-base2"`, `className="btn-secondary shadow-base2"`
:::

::: info Rounded Buttons
Just add an extra class `rounded-[999px]` to the className for a rounded button. For example: `className="btn-primary rounded-[999px]"`, `className="btn-secondary rounded-[999px]"`
:::

::: info Rounded Outline Buttons
Just add an extra class `rounded-[999px]` to the className for a rounded button. For example: `className="btn-outline-success rounded-[999px]"`, `className="btn-outline-secondary rounded-[999px]"`
:::

::: info Icon Buttons
Just add an extra props `icon` to add and icon. For example: `icon="ph-outline:newspaper"`.
You can use `iconPosition="right"` props to move the icon on the right side.
:::

::: info Button Sizes
You can use `className="btn-sm"` props for small button and `className="btn-xl"` for large button.
:::

::: info Disabled Buttons
Just add an extra props `isDisabled` to make a button disabled.
:::

::: info Loading Buttons
Just add an extra props `isLoading` to make a button with loading animation.
:::

::: info Block Buttons
Just add an extra class `block-btn` to the className to make a block button. For example: `className="btn-success lock-btn"`, `className="btn-secondary lock-btn"`
:::

::: info Router Link Buttons
Just add an extra props `link` to add a link to the button. For example: `link="/home"`
:::
