# Installation

DasCode admin template is built using Webpack. Webpack is nicely documented to start. You don't need to install or configure tools like Webpack or Babel. Vite is a new breed of frontend build tooling that significantly improves the frontend development experience.

## Prerequisite

---

- [Node.js](https://nodejs.org/en/) (>= 14.0.0)
- [Yarn](https://yarnpkg.com/en/) (>= 1.5.1)
- [NPM](https://www.npmjs.com/) (>= 5.5.1)

::: details How do I check my node version?
Run below command in your terminal:

```sh
node -v
```

Make sure output version is LTS version.

:::

::: details How do I check my npm version?
Run below command in your terminal:

```sh
npm -v
```

Make sure output version is LTS version.

:::

::: tip
Yarn package manager is recommended
:::

## Step. 1: Getting started

1. Download our DashCode - Admin Dashboard Template from your ThemeForest account.
2. After downloading zip from ThemeForest, select the version that you want to work with. Unzip your selected version in your desired location.
3. Open this folder in console / terminal
4. Run below commands:

   ```sh
   # It will install all packages
   yarn install

   # It will start the development server
   yarn dev
   ```

   ::: warning
   If you are using an older node version and getting errors while installing the app then run the command "yarn install --ignore-engines" command instead of "yarn install"
   :::

5. Open `http://localhost:5173` in your browser

::: tip
If you have any issues regarding installation please follow our guide on [getting support](/getting-started/getting-support.html) for our product.
:::
