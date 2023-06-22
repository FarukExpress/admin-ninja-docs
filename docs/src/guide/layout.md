# Layout

Understanding template layouts will help you create a page with your desired layout.

## Default Layout

The default layout is the layout for all pages which do not require authentication. It is a simple layout that does not include any header, footer, and sidebar.

#### Usage

```jsx
<div>
  <div>
    <main>lorem</main>
  </div>
</div>
```

## App Layout

The app layout is the default layout for all pages which are inside the dashboard. It is a simple layout that includes a header, footer, sidebar, and customizer.

#### Usage

```jsx
import Header from "@/components/partials/Header";
import Footer from "@/components/partials/Footer";
import Sidebar from "@/components/partials/Sidebar";

const Layout = () => {
  return (
    <div>
      <Header />
      <Sidebar />
      <div className="content-wrapper">
        <main>lorem</main>
      </div>
      <Footer />
    </div>
  );
};
```
