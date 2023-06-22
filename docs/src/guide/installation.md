# Installation Guide

To start using the Ninja Admin Template, follow these installation steps:

## Prerequisite

Make sure you have the following tools installed on your system:

- [Node.js](https://nodejs.org/en/) (>= 14.0.0)
- [Yarn](https://yarnpkg.com/en/) (>= 1.5.1)
- [NPM](https://www.npmjs.com/) (>= 5.5.1)

::: details How to check Node.js version
Open your terminal and run the following command:

```sh
node -v
```

Ensure that the displayed version is the LTS version.

:::

::: details How to check NPM version
Open your terminal and run the following command:

```sh
npm -v
```

Ensure that the displayed version is the LTS version.

:::

::: tip
We recommend using the Yarn package manager.
:::

## Getting started

1. Download the Ninja Admin Dashboard Template from your ThemeForest account.
2. Once downloaded, unzip the file and choose the version you wish to work with.
3. Open your desired version's folder in the console or terminal.
4. Run the following commands:

   ```sh
    # Install all the required packages
   yarn install

   # Start the development server
   yarn dev
   ```

   ::: warning
   If you encounter errors during installation due to using an older version of Node.js, use the command "yarn install --ignore-engines" instead of "yarn install".
   :::

5. Open `http://localhost:5173` in your browser

::: tip
If you have any issues regarding installation please follow our guide on [getting support](/getting-started/getting-support.html) for our product.
:::
