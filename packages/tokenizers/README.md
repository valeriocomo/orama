# Orama Tokenizers

This package provides support for additional tokenizers for the Orama Search Engine.

Available tokenizers:
- Chinese (Mandarin - stemmer not supported)
- Japanese (work in progress)
- Korean (work in progress)

Usage:

```js
import { create } from '@orama/orama'
import { createTokenizer } from '@orama/tokenizes/mandarin'

const db = await create({
  schema: {
    myProperty: 'string',
    anotherProperty: 'number'
  },
  components: {
    tokenizer: await createTokenizer()
  }
})
```

# License
[Apache 2.0](/LICENSE.md)