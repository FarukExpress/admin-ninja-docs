# Progress Bar

The progress bar component is a simple progress bar component that can be used to show the progress of any task.

## Basic example

```js
import ProgressBar from "@/components/ProgressBar";

const Example = () => {
  return (
    <div>
      <ProgressBar value={30} className="bg-primary-500" />
      <ProgressBar value={80} className="bg-danger-500" />
      <ProgressBar value={50} className="bg-warning-500" />
      <ProgressBar value={70} className=" bg-info-500" />
    </div>
  );
};
```

::: tip
You can use `className` props for customizing the progress bar.
:::
