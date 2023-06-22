# Modal

Modal is a dialog that appears on top of the main window. It is used to display information or collect user input. It is a component of the [Dialogs](https://headlessui.com/vue/dialog) category.

We have already created several modals. You can use them easily anywhere in the project.

## Basic example

```js
import Modal from "@/components/Modal";
import Button from "@/components/Button";

const Example = () => {
  const [activeModal, setActiveModal] = useState(false);

  return (
    <div>
      <Button
        text="Open Modal"
        btnClass="btn-primary"
        onClick={() => setActiveModal(true)}
      />
      <Modal
        activeModal={activeModal}
        onClose={() => setActiveModal(false)}
        title="Modal Title"
        footer={
          <Button
            text="Close"
            btnClass="btn-primary"
            onClick={() => setActiveModal(false)}
          />
        }
      >
        <h4 className="font-medium text-lg mb-3 text-slate-900">
          Lorem ipsum dolor sit.
        </h4>
        <div className="text-base text-slate-600 dark:text-slate-300">
          Oat cake ice cream candy chocolate cake chocolate cake cotton candy
          dragée apple pie. Brownie carrot cake candy canes bonbon fruitcake
          topping halvah. Cake sweet roll cake cheesecake cookie chocolate cake
          liquorice.
        </div>
      </Modal>
    </div>
  );
};
```

::: warning Note
You can use `activeModal` props for active modal.
`centered` props for centered modal.
`disableBackdrop` props for disabled backdrop.
`noFade` props for disabled fade animation.
`className` props for changing modal size. eg: `className="w-1/2"` for half modal.

:::
