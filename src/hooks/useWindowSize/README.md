# useWindowSize

The custom `useWindowSize` hook is used to watch the window's width during resizing. This allows us to do something based on the width of the screen.

Setup:

- Import it: `import useWindowSize from "./hooks/useWindowSize";` (adjust path as needed)
- Set a variable to the return value of the hook: `const width = useWindowSize();`
- Use as needed

A working example of this can be seen in the `Hero` component. There, we render out a different background SVG for either mobile or tablet + desktop sized screens.
