---
title: compress
description: An extension to compress the body of the response with [Brotli](https://github.com/google/brotli), [gzip](https://www.gzip.org), or [deflate](https://www.ietf.org/rfc/rfc1951.txt), based on the `Accept-Encoding` header of the incoming request.
order: 2
---

Please don't use this extension when you're deploying your app to Deno Deploy or Cloudflare Workers as they handle this for you in a much more optimized way. {.tip}

```ts
import cheetah from 'https://deno.land/x/cheetah/mod.ts'
import { compress } from 'https://deno.land/x/cheetah/ext/compress.ts'

const app = new cheetah()
  .use(compress())
```
