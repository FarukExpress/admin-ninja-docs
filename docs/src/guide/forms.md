# Forms

- [Textinput](#textinput)
- [Textarea](#textarea)
- [Select](#select)
- [Checkbox](#checkbox)
- [Radio](#radio)
- [Switch](#switch)

## Textinput

```js
import Textinput from "@/components/Textinput";

const Example = () => {
  return (
    <div>
      <Textinput
        label="Project Name*"
        name="pn"
        type="text"
        placeholder="Management dashboard "
      />
    </div>
  );
};
```

::: tip
You can use html input attribute via props. For example: `type="text"`, `name="pn"`, `placeholder="Management dashboard"`
You can also use `label` props for label text.
:::
::: warning Note
For label and input connection use `name` props.
You can also make input `horizontal` by using `horizontal` props.
:::

::: tip
Pass `error` & `success` props for error message.

```js
<Textinput
  label="Project Name*"
  name="pn"
  type="text"
  placeholder="Management dashboard "
  error="This field is required"
/>
```

:::

## Textarea

```js
import Textarea from "@/components/Textarea";

const Example = () => {
  return (
    <div>
      <Textarea
        label="Project Description*"
        name="pd"
        placeholder="Write a short description about your project"
      />
    </div>
  );
};
```

::: tip
You can use html textarea attribute via props. For example: `name="pd"`, `placeholder="Write a short description about your project"`
You can also use `label` props for label text.
:::
::: warning Note
For label and textarea connection use `name` props.
You can also make textarea `horizontal` by using `horizontal` props.
Pass `error` & `success` props for error message.

:::

## Select

```js
import Select from "@/components/Select";
const options = [
  { value: "1", text: "Web Application" },
  { value: "2", text: "Mobile Application" },
  { value: "3", text: "Desktop Application" },
  { value: "4", text: "Other" },
];

const Example = () => {
  return (
    <div>
      <Select
        label="Project Type*"
        name="pt"
        placeholder="Select project type"
        options={options}
      />
    </div>
  );
};
```

::: tip
You can use html select attribute via props. For example: `name="pt"`, `placeholder="Select project type"`
You can also use `label` props for label text.
:::

::: warning Note
For label and select connection use `name` props.
For Horizontal select use `horizontal` props.
:::

## Checkbox

```js
import Checkbox from "@/components/Checkbox";

const Example = () => {
  const [checked, setChecked] = useState(false);
  return (
    <div>
      <Checkbox
        label="Checked"
        value={checked}
        onChange={() => setChecked(!checked)}
      />
    </div>
  );
};
```

## Radio

```js
import Radio from "@/components/Radio";

const Example = () => {
  const [value, setValue] = useState("A");
  const [value2, setValue2] = useState("C");
  const handleChange = (e) => {
    setValue(e.target.value);
  };
  return (
    <div>
      <Radio
        label="Checked"
        name="x"
        value="A"
        checked={value === "A"}
        onChange={handleChange}
      />
      <Radio
        label="UnChecked"
        name="x"
        value="B"
        checked={value === "B"}
        onChange={handleChange}
      />
    </div>
  );
};
```

## Switch

```js
import Switch from "@/components/Switch";

const Example = () => {
  const [checked, setChecked] = useState(false);
  return (
    <div>
      <Switch
        label="Active Switch"
        value={checked}
        onChange={() => setChecked(!checked)}
      />
    </div>
  );
};
```
