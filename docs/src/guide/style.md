# Style Tailwindcss

## Introduction

Tailwindcss is a utility-first CSS framework for rapidly building custom user interfaces. It is a highly customizable, low-level CSS framework that gives you all of the building blocks you need to build bespoke designs without any annoying opinionated styles you have to fight to override.

## Installation

```bash
npm install -D tailwindcss@latest postcss@latest autoprefixer@latest
```

## Configuration

```bash
npx tailwindcss init
```

## Usage

```jsx
const App = () => {
  return (
    <div className="bg-gray-200">
      <div className="bg-white shadow overflow-hidden sm:rounded-lg">
        <div className="px-4 py-5 sm:px-6">
          <h3 className="text-lg leading-6 font-medium text-gray-900">
            Profile
          </h3>
          <p className="mt-1 max-w">
            This information will be displayed publicly so be careful what you
            share.
          </p>
        </div>
      </div>
    </div>
  );
};
```

## Configuration

```js
// tailwind.config.js
module.exports = {
  purge: ["./src/**/*.{js,jsx,ts,tsx}", "./public/index.html"],
  darkMode: false, // or 'media' or 'className'
  theme: {
    extend: {},
  },
  variants: {
    extend: {},
  },
  plugins: [],
};
```
