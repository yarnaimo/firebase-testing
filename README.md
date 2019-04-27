```ts
import { FirestoreTest } from '@yarnaimo/firebase-testing'

const provider = new FirestoreTest('name')

beforeEach(async () => {
    provider.next()
    await provider.loadRules()
})

afterEach(async () => {
    await provider.cleanup()
})
```
