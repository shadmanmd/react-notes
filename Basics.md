# Clean Boilerplate

Delete everything inside src folder, except index.js

# ReactDom

It has a render function which takes two arguments - the component and the location where the component must be rendered inside public/index.html

```javascript
import ReactDom from "react-dom";
ReactDom.render(<Greeting />, document.getElementById("root"));
```
