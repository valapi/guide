# Usage

-----------

```typescript
import Client from '@valapi/auth';
```

## [Client](./Client.md#client)

```typescript
const AuthClient = new Client();
```

## [Auth](./Auth.md#basic-authentication)

```typescript
await AuthClient.login('BestUsername', 'SuperSecretPassword');
```

```typescript
if (AuthClient.multifactor === true) {

    await AuthClient.verify(428793 /* <--- Verify Code */);
    
}
```

## PlayerUUID (puuid)

```typescript
const puuid = AuthClient.parsePlayerUuid();
```