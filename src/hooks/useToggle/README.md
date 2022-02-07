# useToggle

The custom `useToggle` hook is to be used when you simply want to flip a boolean state between true or false. The hook returns 2 elements:

- The value (state, of type boolean)
- State updating function

So, it is quite similar to the `useState` hook, and can be used in a very similar, if not identical, manner.

Setup:

- Import it: `import useToggle from "./hooks/useToggle";` (adjust path as needed)
- Destructure the two elements the hook returns: `const [toggle, setToggle] = useToggle();`
- Use the boolean value for a prop, for example: `isOpen={toggle}`
- Call the state updating function where needed to flip the state: `onClick={setToggle}`

A working example of this can be seen in the `AvailablePositions` component. There, we simply toggle the `FilterDropdown` styled component open and close.
