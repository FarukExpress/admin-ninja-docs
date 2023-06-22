# Card

Card is a flexible and extensible content container. It includes options for headers and footers, a wide variety of content, contextual background colors, and powerful display options.

## Basic example

```js
import Card from "@/components/Card";
const ExamplePage = () => {
  return (
    <Card title="Card title" subtitle="This is a subtitle">
      Lorem ipsum dolor sit amet, consec tetur adipiscing elit, sed do eiusmod
      tempor incididun ut .
    </Card>
  );
};
```

::: tip You can use `className` props for custom class. For example: `className="bg-primary-500"`, `className="bg-secondary-500"`, `className="bg-success-500"`, `className="bg-danger-500"`, `className="bg-warning-500"`, `className="bg-info-500"`,
:::
