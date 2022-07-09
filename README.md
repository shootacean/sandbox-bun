# sandbox-bun

[Bun is a fast all-in-one JavaScript runtime](https://bun.sh/) sandbox.

## Quick  start

```shell
# Install
curl https://bun.sh/install | bash

# create server.js
touch http.js
```

```js
// http.js
export default {
  port: 3000,
  fetch(request) {
    return new Response("Welcome to Bun!");
  },
};
```

```shell
bun run http.js
```

```shell
curl localhost:3000
Welcome to Bun!
```
