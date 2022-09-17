# Example

-----------

```typescript
import { Client } from '@valapi/api-wrapper';
```

## [Client](./Client.md#client)

```typescript
const ApiClient = new Client({
    region: 'ap',
});
```

## [Auth](../../PACKAGE/auth/Auth.md)

```typescript
await ApiClient.login('BestUsername', 'SuperSecretPassword');
```

```typescript
if(ApiClient.isMultifactor === true) {

    await ApiClient.verify(428793 /* <--- Verify Code */);
    
}
```

## [API](./API.md#usage)

```typescript
const _data = await ApiClient.PreGame.getMatch('MATCH-ID-1234567890');

console.log(_data.data);
```