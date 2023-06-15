# GPollet Dropdown

A React component using Typescript to create a dropdown menu from a list of items.

## Installation

To install the latest version using npm :

```bash
  npm install gpollet-dropdown
```

To install the latest version using Yarn :

```bash
  yarn add gpollet-dropdown
```

## Usage/Examples

Component can be used as a regular React component once imported into a file.

### Props

All props are typed using Typescript.

| Prop Name | Role                                                                        | Type             | Required |
| --------- | --------------------------------------------------------------------------- | ---------------- | -------- |
| data      | Values to display as < option/>{string}</ option> in the dropdown menu      | {name: string}[] | x        |
| label     | Text content of the <label> tag.                                            | string           | x        |
| id        | Id that will be assigned to the <select> tag.                               | string           | x        |
| name      | Name that will be assigned to the <select> tag. <br> _Default value : {id}_ | string           |          |
| width     | Width of the <select> element. <br> _Default value : 300_                   | number           |          |
| height    | Height of the <select> element.<br> _Default value : 300_                   | number           |          |

```javascript
import Dropdown from "gpollet-dropdown";

function App() {
	return (
		<>
			<div className="App">
				<Dropdown
					data={[
						{ name: "Option A" },
						{ name: "Option B" },
						{ name: "Option C" },
					]}
					label="Dropdown Example"
					id="dropdown-id"
				/>
			</div>
		</>
	);
}

export default App;
```
