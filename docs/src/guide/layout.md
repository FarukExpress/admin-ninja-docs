# Layout

Understanding the different layouts used in a template can help you create pages with your desired structure and design.

## Auth Layout

The default layout is used for pages that do not require authentication. It is a simple layout without a header, footer, or sidebar.

### Usage

```jsx
const AuthLayout = () => {
  return (
    <div>
      <div>
        <main>{/* Content goes here */}</main>
      </div>
    </div>
  );
};
```

## App Layout

The app layout is the default layout for pages within the dashboard. It includes a header, footer, sidebar, and customizer.

#### Usage

```jsx
import Header from "@/components/partials/Header";
import Footer from "@/components/partials/Footer";
import Sidebar from "@/components/partials/Sidebar";

const AppLayout = () => {
  return (
    <div>
      <Header />
      <Sidebar />
      <div className="content-wrapper">
        <main>{/* Content goes here */}</main>
      </div>
      <Footer />
    </div>
  );
};
```
