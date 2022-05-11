# Example

-----------

```typescript
import { Client } from '@valapi/riot-api';
```

## Client

```typescript
const ApiClient = new Client({
    language: 'en-US',
});

```

## API

```typescript
const _data = await ApiClient.AccountV1.ByRiotId('PRX f0rsakeN', 'Huh');

console.log(_data.data);
```