# JSX (JavaScript XML) Rules

- Return a single element.
- We can wrap everything in div / section / article or Fragment.

  - Fragment is a tag written as

    ```javascript
    <React.Fragment></React.Fragment>
    // or just opening & closing angular brackets
    <></>
    ```

- Use camelCase for HTML attributes.
- Use 'className' instead of 'class'.
  - since class is already a keyword in ES6.
- Every element must have a closing tag.

# JSX inline CSS

- The style attribute is added in an HTML tag in the JS file as a JavaScript object.
- The values are written in quotes as it is a JavaScript object.

  - Eg:

  ```javascript
  <h4
    style={{
      color: "red",
    }}
  ></h4>
  ```

# JavaScript in JSX

- Enclosed in curly brackets
- It must return a value

  - Eg:

  Correct way

  ```javascript
  const title = 'The Family Man'
  <p>{title}</p>
  ```

  Wrong way

  ```javascript
  <p>{const title = 'The Family Man'}</p>
  ```
