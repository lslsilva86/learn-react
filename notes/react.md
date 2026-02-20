# What React Can Do (React 19)

## Core UI Building
React lets you build component-based UIs using JSX, compose components together, and manage local state with hooks like `useState` and `useReducer`.

## Rendering
It supports client-side rendering (CSR), server-side rendering (SSR), and static site generation (SSG) — typically via frameworks like Next.js or Remix. React 19 also introduced improved support for React Server Components (RSC), letting you render components entirely on the server with zero client-side JS.

## State Management
Built-in hooks cover most needs: `useState`, `useReducer`, `useContext`. For global state, you can integrate libraries like Redux, Zustand, Jotai, or Recoil.

## Side Effects & Lifecycle
`useEffect` handles side effects. `useLayoutEffect` runs synchronously after DOM mutations. `useInsertionEffect` is for CSS-in-JS libraries.

## Performance Optimization
`useMemo` and `useCallback` memoize values and functions. `React.memo` prevents unnecessary re-renders. The React Compiler (introduced experimentally in React 19) can auto-memoize components. `useTransition` and `useDeferredValue` let you mark updates as non-urgent to keep the UI responsive.

## Concurrent Features
React's concurrent mode allows it to pause, resume, and prioritize rendering work. This powers `Suspense` for lazy loading and data fetching, and `useTransition` for smooth UI updates.

## Data Fetching (React 19)
React 19 introduced the `use()` hook, which lets you read promises and context directly in render. It also introduced built-in support for `<form>` actions and server actions (via frameworks), making form handling and mutations much simpler.

## Refs & DOM Access
`useRef` gives you direct DOM access or a mutable container. React 19 simplified ref handling — you can now pass `ref` as a regular prop instead of needing `forwardRef`.

## Error Handling
Error Boundaries catch rendering errors in subtrees. React 19 added improved error reporting and new hooks like `useOptimistic` for optimistic UI updates.

## Portals
`ReactDOM.createPortal` lets you render children into a DOM node outside the parent hierarchy — useful for modals and tooltips.

## Animations
React integrates well with Framer Motion, React Spring, and CSS transitions. No built-in animation system, but the architecture supports it cleanly.

## Cross-Platform
Via React Native, the same component model extends to iOS and Android apps. React Native for Web brings it back to browsers.

## Developer Tooling
React DevTools (browser extension) lets you inspect component trees, profile renders, and debug state.

---

> In short, React is primarily a UI rendering library, but its ecosystem and React 19's new primitives push it closer to a full-stack framework primitive — especially when paired with a meta-framework like Next.js.
