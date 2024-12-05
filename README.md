# React Keyboard

Made the `App` a class component with `pressedKey` in the `state`.

- before any key was pressed show the `Nothing was pressed yet` message;
- when a key is pressed show a `The last pressed key is [key]` message;
- use `componentDidMount` to add `keyup` handler:
    ```ts
    // DON'T import KeyboardEvent from React, because it is a regular event
    document.addEventListener('keyup', (event: KeyboardEvent) => {
      console.log(event.key);
    });
    ```
- use `removeEventListener` to remove a global handler in `componentWillUnmount`.

## Demo Links

- [DEMO LINK](https://AndriiZakharenko.github.io/react_keyboard/)
