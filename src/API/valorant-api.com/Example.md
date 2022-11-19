# Example

-----------

```typescript
import { Client } from '@valapi/valorant-api.com';
```

## [Client](./Client.md#config)

```typescript
const ApiClient = new Client({
    language: 'en-US',
});

```

## [API](./API.md#usage)

```typescript
const data = await ApiClient.Events.get();

console.log(data.data);
```