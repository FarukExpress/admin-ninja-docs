# Alert

Alert is a component that displays a message to the user.

## Theme Color Alerts

```jsx
import Alert from "@/components/Alert";
const Page = () => {
  return(
    <div>
      <Alert
        label="This is an alert—check it out!"
        className="alert-primary"
      />

    </div>
  )
}
</script>
```

::: tip
You can use `className` for alert type. Available types: `className="alert-primary"`, `className="alert-secondary"`, `className="alert-success"`, `className="alert-info"`, `className="alert-danger"`, `className="alert-warning"`,
:::

::: tip Light Color Alerts
Just add `light` to the type. For example: `className:light-mode alert-primary`;
:::

::: tip Outline Alerts
Just add `outline` to the type. For example: `className:alert-outline-primary`;
:::

::: tip Dismissible
You can use `dismissible` props to make an alert dismissible.
:::

::: tip Icon
You can use `icon="fluent:target-20-regular` props to add an icon on the alert component.
:::
