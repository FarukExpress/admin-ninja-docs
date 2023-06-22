# Navigation Menu

Learn how to add navigation items to the vertical and horizontal menus.

- [Vertical Menu](#verticalmenu)
- [Horizontal Menu](#horizontalmenu)

## Vertical Menu

To add a navigation item to the vertical menu, follow these steps:

1. Open the `mocks/data.js` file.

2. Locate the menuItems array.

3. Add a new item to the array with the following properties:

- `title`: The title of the menu item.
- `icon`: The icon for the menu item (you can use Phosphor for icons).
- `link`: The route name from the App.jsx file that the menu item should link to.

#### Example:

```js
{
  title: "Chat",
  icon: "heroicons-outline:chat",
  link: "chat",
}
```

::: warning Note
The `link` property should correspond to a route name defined in the `App.jsx` file.
:::

::: tip Tip
Remember, you can customize the icons by choosing from the available options in [Phosphor](https://iconify.design/).

:::

::: details Adding a Menu Label
To add a menu label, include a new item in the menuItems array with the label property.

```js
{
  isHeader: true,
  title: "DASHBOARD",
}
```

:::

::: details Adding Sub Menu Items
To add sub menu items, follow these steps

1. Add a new child property to the parent item object in the menuItems array.
2. Within the child array, define each sub menu item using the childtitle and childlink properties.

```js
{
    title: "Dashboard",
    icon: "ph-outline:home",
    isOpen: true,
    child: [
        {
        childtitle: "Analytics Dashboard",
        childlink: "home",
        },
        {
        childtitle: "Ecommerce Dashboard",
        childlink: "ecommerce",
        },
    ],
},
```

::: warning Note
The `childlink` property should correspond to a route name defined in the router.js file. To have a sub menu item open by default, include the isOpen: true property in the parent item object.

:::

## Horizontal Menu

To add a navigation item to the horizontal menu, follow these steps:

1. Open the `mocks/data.js` file.

2. Locate the menuItems array.

3. Add a new item to the array with the following properties:

- `title`: The title of the menu item.
- `icon`: The icon for the menu item (you can use Phosphor for icons).
- `link`: The route name from the App.jsx file that the menu item should link to.

#### Example:

```js
export const topMenu = [
  {
    title: "Chat",
    icon: "ph-outline:chat",
    link: "chat",
  },

  {
    title: "Email",
    icon: "ph-outline:mail",
    link: "email",
  },

  {
    title: "Kanban",
    icon: "ph-outline:view-boards",
    link: "kanban",
  },
];
```

::: warning Note
The `link` property should correspond to a route name defined in the `router.js` file.
:::

::: tip Tip
You can use [iconify](https://iconify.design/) for icons.
:::

::: details How I add sub menu items?
you can add sub menu items by adding a new `child` property in the item object.

```js
export const topMenu = [
  {
    title: "Dashboard",
    icon: "ph-outline:home",
    isOpen: true,
    child: [
      {
        childtitle: "Analytics Dashboard",
        childlink: "home",
      },
      {
        childtitle: "Ecommerce Dashboard",
        childlink: "ecommerce",
      },
    ],
  },
];
```

::: warning Note
The `childlink` property should a route name from `router.js` file.
:::
