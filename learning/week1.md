# Redux and Prop Passing

With Redux, you don’t need to pass props down through many components (prop drilling). Any component can access or update the shared state directly from the Redux store using hooks like `useSelector` and `useDispatch`. This makes your code cleaner and easier to manage, especially in large apps.

**Summary:**

- Redux keeps all important app data in one central place (the store).
- Components can read or update this data without passing it through many layers.
- This avoids messy prop passing and makes state management predictable and centralized.

---

## Overlay Layout: relative and absolute

To create overlays (like a dark layer or centered text on top of an image), use:

This lets you stack and position elements exactly where you want inside the parent, which is essential for hero sections, modals, and custom UI layers.

## Animation with framer-motion

framer-motion lets you animate React components easily. You define animation states (like `hidden` and `visible`) and set how elements should animate between them.

**Common flow:**

- The container (e.g., `<motion.div>`) starts in a `hidden` state (like opacity: 0, y: 50).
- When it comes into view, it animates to `visible` (opacity: 1, y: 0).
- `staggerChildren` in the container's transition makes each child animate in sequence, not all at once.
- Each child (e.g., `<motion.h2>`, `<motion.div>`) uses its own variants for entrance effects (like fading in and moving up).
- The layout (CSS/grid/flex) sets the final position; the animation just moves/fades the element into place.

This creates smooth, coordinated entrance animations for sections and their content.

inset-0 is a Tailwind CSS class that sets top: 0, right: 0, bottom: 0, and left: 0 for an absolutely positioned element.