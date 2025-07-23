# Redux and Prop Passing

With Redux, you don’t need to pass props down through many components (prop drilling). Any component can access or update the shared state directly from the Redux store using hooks like `useSelector` and `useDispatch`. This makes your code cleaner and easier to manage, especially in large apps.

**Summary:**

- Redux keeps all important app data in one central place (the store).
- Components can read or update this data without passing it through many layers.
- This avoids messy prop passing and makes state management predictable and centralized.
