# Example

-----------

```typescript
import { Client } from '@valapi/riot-api';
```

## [Client](./Client.md#config)

```typescript
const ApiClient = new Client({
    language: 'en-US',
});

```

## [API](./API.md#usage)

```typescript
const _data = await ApiClient.Events.get();

console.log(_data.data);
```