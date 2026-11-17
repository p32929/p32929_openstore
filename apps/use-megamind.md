---
title: use-megamind
icon: screenshots/use-megamind/icon.png
screenshots:
  - screenshots/use-megamind/1.png
category: Developer Tools
summary: Small React hook for async calls. Get data, error and loading state for any async function, a lightweight alternative to React Query
tags: [React hook, Async, Data fetching, React Query alternative, Loading state, Next.js, TypeScript, npm]
website: https://github.com/p32929/use-megamind
source: https://github.com/p32929/use-megamind

platforms:
  Library: https://www.npmjs.com/package/use-megamind
---

use-megamind is a small React hook for calling async functions on the client side. Most of the time you only want the data, the error and a loading flag, and writing the same `useState` and `useEffect` code for every call gets tiring. React Query does it, but it takes a lot of reading to start. Give use-megamind any async function and it gives you `data`, `error` and `isLoading`.

I made it because React Query is awesome, but it has a lot of things I didn't need. I just needed something simple, so I made it.

1. **Any async function,** not only data fetching, with or without parameters.
2. **Call it right away or later,** for example on a button click.
3. **Options when you need them:** limit how many times it can be called, set a minimum delay between calls, cache the result until the page reloads, and turn on debug logs.
4. **Append data:** add newly fetched data to what you already have, handy for "load more" lists.
5. **Callbacks and checks:** run code on success or error, and set checks once for every hook in the app.

Great for React and Next.js apps that want simple async state without a big library.

## Install

```bash
npm install use-megamind
```

```tsx
const { data, error, isLoading } = useMegamind(myAsyncFunction)
```

Want to buy the source code of this app? Contact me through my portfolio: https://p32929.github.io
