# Button

Button is a component that can be used to trigger an action or event, such as submitting a form, opening a dialog, canceling an action, or performing a delete operation.

### Use

```js
import Button from "@/components/Button";
const ButtonPage = () => {
  return (
    <div>
      <Button text="primary" className="btn-primary" />
      <Button text="primary" className="btn-primary rounded-[999px] " />
      <Button text="primary" className="btn-primary light" />
      <Button icon="ph:pentagram" text="Right Icon" className="btn-secondary" />
    </div>
  );
};
```

::: tip Button Props
You can use `className`, `isLoading`, `isDisabled`, `icon` .
:::

::: tip className
`btn-primary`, `btn-secondary`, `btn-info`, `btn-danger`, etc you can also pass
class name like `bg-blue-500 text-white` this.
:::
