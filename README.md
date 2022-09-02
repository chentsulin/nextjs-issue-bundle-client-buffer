# nextjs-issue-bundle-client-buffer

## Demo

```bash
ANALYZE=true yarn build
```

Before:

![](https://user-images.githubusercontent.com/3382565/188085102-107f5ef9-52e6-43ae-b07f-db4aab70d84e.png)


After adding a `typeof Buffer` check to `pages/index.js`:

```js
const isNode = typeof Buffer !== 'undefined';
console.log({ isNode });
```

![](https://user-images.githubusercontent.com/3382565/188085134-6786613e-49e3-43e5-9cf0-e1d68aec3c67.png)