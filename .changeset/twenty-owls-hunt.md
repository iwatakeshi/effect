---
"effect": minor
---

Schema: Add `standard` API to Generate a [Standard Schema v1](https://standardschema.dev/).

**Example**

```ts
import { Schema } from "effect"

const schema = Schema.Struct({
  name: Schema.String
})

//      ┌─── StandardSchemaV1<{ readonly name: string; }>
//      ▼
const standardSchema = Schema.standard(schema)
```
