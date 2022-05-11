# Example

-----------

```typescript
import { Client } from '@valapi/riot-api';
```

## Client

```typescript
const ApiClient = new Client({
    apiKey: 'LoooooongApiKey_123456789',
    region: 'ap',
});

```

## API

```typescript
const _data = await ApiClient.AccountV1.ByRiotId('PRX f0rsakeN', 'Huh');

console.log(_data.data);
```