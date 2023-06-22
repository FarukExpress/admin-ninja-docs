# How to create a new page

Just create a new `.js/jsx` file in `src/views` folder. For example you can use `src/about.jsx`.

::: warning
If you want to create a new page then you need to add the page to the `src/App.jsx` file.
:::

### Creating a new page

Create a new `.js/jsx` file in the `src/pages` folder. You can use `src/about.jsx`.
and add the page to the `src/App.js` file. in `Layout` component.

```js
const About = () => {
  return (
    <div class="about">
      <h1>About</h1>
    </div>
  );
};
```

```js
<Routes>
  <Route path="/" element={<Layout />}>
    <Route path="/about" element={<About />} />
  </Route>
</Routes>
```

### Adding a new page to the sidebar

Go to `src/constant` file and add the page to the `menuItems` array.

```js
{
    title: "About",
    icon: "ph-outline:user",
    link: "email",
},

```
