# Example

-----------

```typescript
import { ValRso } from '@valapi/auth';
```

## [Client](./Client.md#client)

```typescript
const AuthClient = new ValRso();
```

## [Auth](./Auth.md#basic-authentication)

```typescript
await AuthClient.login('BestUsername', 'SuperSecretPassword');
```

```typescript
if(AuthClient.multifactor === true) {

    await AuthClient.verify(428793 /* <--- Verify Code */);
    
}
```

```typescript
const _data = AuthClient.toJSON();

const AuthClient = await ValRso.fromCookie(_data.cookie.ssid);
```