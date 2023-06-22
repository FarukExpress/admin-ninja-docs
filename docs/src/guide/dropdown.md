# Dropdown

Dropdown is a component that can be used to Toggle contextual overlays for displaying lists of links and more with the dropdown plugin.

## Basic Dropdown

```js
import Dropdown from "@/components/Dropdown";

const menus = [
  {
    label: "Action",
    link: "#",
  },
  {
    label: "Another action",
    link: "#",
  },
  {
    label: "Something else here",
    link: "#",
  },
  {
    label: "Separated link",
    link: "#",
    hasdivider: true,
  },
];
const ExamplePage = () => {
  return (
    <div>
      <Dropdown label="Basic Dropdown" items={menus} />
    </div>
  );
};
```

::: details How Can I use Custom Label?
You can also use `Button` component as a label. or any text or html element.

##### Example for Button Component

```js
<Dropdown label={
    <Button
    text="Custom Label"
    btnClass="btn-primary"
    icon="heroicons-outline:chevron-right"
    iconPosition="right"
    div
    iconClass="text-lg"
  />
}>
```

You can use all props of [Button](button.html) component.

##### Example For Custom Text

```js
<Dropdown label={<span>Custom Label</span>} />
```

:::

::: details How Can I use dropdown options as like a menu items?

```js
<Dropdown
  label={
    <Button
      text="Custom Label"
      btnClass="btn-primary"
      icon="heroicons-outline:chevron-right"
      iconPosition="right"
      div
      iconClass="text-lg"
    />
  }
>
  <div class="single-menu-item">single menu one</div>
  <div class="single-menu-item">single menu two</div>
  <div class="single-menu-item">single menu three</div>
</Dropdown>
```

:::
::: warning All Classes for Dropdown
You can use `classMenuItems` props for dropdown direction type. Available types: Left Align: `classMenuItems="left-0  w-[220px] top-[110%]"`,

Right Align: `classMenuItems="right-0  w-[220px] top-[110%]"`

Label class: `labelClass="btn-primary"`

Parent class: `parentClass="relative"`

:::

## Split Dropdown

```js
import SplitDropdown from "@/components/Dropdown/SplitDropdown";
const menus = [
  {
    label: "Action",
    link: "#",
  },
  {
    label: "Another action",
    link: "#",
  },
  {
    label: "Something else here",
    link: "#",
  },
  {
    label: "Separated link",
    link: "#",
    hasdivider: true,
  },
];

const ExamplePage = () => {
  return (
    <div>
      <SplitDropdown label="Split Dropdown" items={menus} />
    </div>
  );
};
```

::: tip Tip
All options and classes and slot are same as Dropdown component.
:::

```

```
