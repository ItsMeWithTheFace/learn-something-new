# Jest

- a flexible javascript testing framework
- used to test different UIs

## Snapshot testing
- Render your app at a high level (snapshot)
    - example
    ```javascript
    exports[`renders correctly 1`] = `
    <a
      className="normal"
      href="http://www.facebook.com"
      onMouseEnter={[Function]}
      onMouseLeave={[Function]}
    >
      Facebook
    </a>
    `;
    ```
- check inconsistencies such as links or pictures being incorrect
- snapshots should be committed alongside code


