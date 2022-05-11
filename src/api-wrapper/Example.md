# Example

-----------

```typescript
import { Client } from '@valapi/api-wrapper';
```

## Client

```typescript
const ApiClient = new Client({
    region: 'ap',
});

```

## Auth

```typescript
await ApiClient.login('BestUsername', 'SuperSecretPassword');

if(ApiClient.multifactor === true) {

    //multifactor
    await ApiClient.verify(428793);
}
```

## API

```typescript
const _data = await ApiClient.PreGame.GetMatch('MATCH_ID');

console.log(_data.data);
```