# Folder Structure React Js

Understand the folder structure of the template and what the template contains.

## Step-1 : Root Structure

The `root` folder contains the core code of this application. The DashCode folder structure looks like this.

```
.
├─ src
│  ├─ assets
│  │  ├─ images
│  │  ├─ scss
│  ├─ components
│  │  ├─ partials
│  │  ├─ ui
│  │  ├─ widgets
│  ├─ constant
│  |  ├─ data.js
│  |  ├─ appex-chart.js
│  |  ├─ chartjs-data.js
│  |
│  ├─ config
│  ├─ Layout
│  ├─ hooks
│  ├─ store
│  ├─ pages
│  │  ├─ dashboard
│  │  ├─ components
│  │  ├─ chart
|  |- App.jsx
│  ├─ main.jsx
|
├─ favicon.svg
├─ index.html
├─ .gitignore
├─ package.json
├─ README.md
|- postcss.config.js
|- tailwind.config.js
|- vite.config.js
│
│
└─ package.json
```

## Step-2 : Assets

The assets folder contains logos and other static assets. You can place your static assets here.

## Step-3 : Components

Place your components in the `components` folder. Each component should be placed in its own folder. The folder name should be the name of the component.

```

├─ Components
│  ├─ partials
│  │  ├─ Header
│  │  │  ├─ index.jsx
│  │
│  ├─ ui
│  │  ├─ Button
│  │  ├─ Card
│  │  ├─ Dropdown
```

::: details How do I use components?
In your `App.js` file, you can import your components like this:

```js
import Button from "@/components/ui/Button";
import Card from "@/components/ui/Card";

const App = () => {
  return (
    <div>
      <Button />
      <Card />
    </div>
  );
};
```

:::

## Step-4 : Layout

The `Layout` folder contains the layouts of this application. You can place any new layout here.

## Step-6 : Pages

The `pages` folder contains the views of this application. You can place new views here.

## Step-7 : Store

The store folder contains the redux-toolkit store files of this application. You can use this folder to store your redux-toolkit files.

## Step-8 : Constants

Define your constants in the `constants` folder. You can place your constants here.
