# useScroll

The custom `useScroll` hook is a combination of the `useInView` hook from [React Intersection Observer](https://github.com/thebuilder/react-intersection-observer), and the `useAnimation` hook from [Framer Motion](https://github.com/framer/motion). This hook allows us to animate elements into view as we scroll past them. We use this hook because Framer Motion does not support this type of animation out of the box. Framer Motion is also a very powerful and popular animation library for React, so we can leverage it in other places if need be.

Setup:

- Import it: `import useScroll from "./hooks/useScroll";` (adjust path as needed)
- Destructure the two elements the hook returns: `const [element, controls] = useScroll();`
- On the Styled Component, set it to: ` styled(motion.div)``; ` (adjust element as needed)
- Import whichever animation you want to use from the `animations` folder: `import { fadeInUp } from "./animations/animations";` (adjust path as needed)
- On the element you wish to animate, add the following props: `animate={controls} initial="hidden" ref={element} variants={fadeInUp}` (adjust the `variants` value to whichever animation you are using)

A working example of this can be seen in the `Banner` component (numerous components use this setup, but the `Banner` component is a small and simple one, therefore it should be easier to read and understand).
