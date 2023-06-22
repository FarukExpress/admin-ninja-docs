# Progress Bar

The progress bar component is a simple progress bar component that can be used to show the progress of any task.

### use

```js
import ProgressBar from "@/components/ProgressBar";

const Example = () => {
  return (
    <div>
      <ProgressBar value={30} className="bg-blue-500" />
      <ProgressBar value={50} className=" bg-fuchsia-500" />
      <ProgressBar value={70} className=" bg-green-500" />
      <ProgressBar value={80} className=" bg-cyan-500" />
      <ProgressBar value={90} className="bg-yellow-500" />
      <ProgressBar value={95} className=" bg-red-500" />
    </div>
  );
};
```

::: tip
You can use `className` props for customizing the progress bar.
:::
