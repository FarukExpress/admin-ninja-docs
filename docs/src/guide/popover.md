# Tooltip

A tooltip is often used to specify extra information about something when the user moves the mouse pointer over an element.

## Tooltip Example

```js
import Tooltip from "@/components/Tooltip";
const Examaple = () => {
  return (
    <Tooltip
      title="Tooltip on top"
      content="Tooltip on top!"
      placement="top"
      className="btn btn-outline-dark "
      theme="primary"
      arrow
    />
  );
};
```

# Popover

Popovers are overlays that open on demand and is mainly used on elements to display more content on floating card popped by clicking or hovering.

## Popover Example

```js
import Tooltip from "@/components/Tooltip";
const Example = () => {
  return (
    <Tooltip
      title="Popover right"
      placement="right"
      className="btn btn-outline-dark"
      arrow
      allowHTML
      interactive
      theme="custom-light"
      maxWidth="320px"
      content={
        <div className="dark:text-slate-300 text-slate-600 text-sm">
          <h1 className="text-base bg-slate-900 dark:bg-slate-600 dark:bg-opacity-70 text-white rounded-t px-[9px] mt-[-5px] mx-[-9px] mb-3 py-2">
            Popover Right
          </h1>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptas reprehenderit
          doloremque mollitia esse eveniet dolor. Eos quasi amet, assumenda omnis
          aliquid cum tenetur ratione tempore similique, itaque maiores et vel.
        </div>
      }
    />
  );
};
```
