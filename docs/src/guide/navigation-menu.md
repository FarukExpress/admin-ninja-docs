# Navigation Menu

In this page you will learn how to add navigation items in vertical navigation & horizontal navigation.

- [Vertical Menu](#verticalmenu)
- [Horizontal Menu](#horizontalmenu)

## Vertical Menu {#verticalmenu}

In order to add a navigation item in vertical menu, you need to add a new item in `menuItems` array in `constant/data.js` file.

```js
export const menuItems = [
  {
    title: "Chat",
    icon: "heroicons-outline:chat",
    link: "chat",
  },

  {
    title: "Email",
    icon: "heroicons-outline:mail",
    link: "email",
  },

  {
    title: "Kanban",
    icon: "heroicons-outline:view-boards",
    link: "kanban",
  },
];
```

::: warning Note
The `link` property should a route name from `App.jsx` file.
:::

::: tip Tip
You can use [Heroicons](https://iconify.design/) for icons.
:::

::: details How to add a menu label?
You can add a menu label by adding a new item in `menuItems` array with `label` property.

```js
{
    isHeadr: true,
    title: "DASHBOARD",
},
```

:::

::: details How I add sub menu items?

You can add sub menu items by adding a new `child` property in the item object.

```js
{
    title: "Dashboard",
    icon: "heroicons-outline:home",
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
The `childlink` property should be the same as the route name in `router.js` file.
If you want to open the sub menu by default, you need to add `isOpen: true` property in the parent item object.

:::

## Horizontal Menu {#horizontalmenu}

In order to add a navigation item in horizontal menu, you need to add a new item in `topMenu` array in `constant/data.js` file.

```js
export const topMenu = [
  {
    title: "Chat",
    icon: "heroicons-outline:chat",
    link: "chat",
  },

  {
    title: "Email",
    icon: "heroicons-outline:mail",
    link: "email",
  },

  {
    title: "Kanban",
    icon: "heroicons-outline:view-boards",
    link: "kanban",
  },
];
```

::: warning Note
The `link` property should a route name from `router.js` file.
:::

::: tip Tip
You can use [Heroicons](https://iconify.design/) for icons.
:::

::: details How I add sub menu items?
you can add sub menu items by adding a new `child` property in the item object.

```js
export const topMenu = [
  {
    title: "Dashboard",
    icon: "heroicons-outline:home",
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
