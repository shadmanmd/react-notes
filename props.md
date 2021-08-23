# Props

- They are the arguments to components
- Example

```javascript
const App() {
  return(
    <div>
      <Employee title="System Engineer" salary={7} />
      <Employee salary={9} />
    </div>
  )
}

const Employee = (props) => {
  return <h1>{props.title}</h1>
}
```

In the output only System Engineer is displayed as for the second component we don't have a title passed.
So, it's not an error.

> We can use object destructuring instead of the dot (.) operator to access props.
>
> ```javascript
> const Employee = ({ title, salary }) => {
>   return <h1>{title}</h1>;
> };
> ```

## Children Props

- Any content inside the opening and closing tags of a component is a children prop. It is special and can be accessed by using the word _children_ inside the component.

- Example

```javascript
<Employee title="System Engineer" salary={7}>
  <p> This paragraph is a children prop. </p>
</Employee>;

const Employee = (props) => {
  return <h1>{props.children}</h1>;
};
```
