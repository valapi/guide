# Example

---

```typescript
import { AuthClient } from "@valapi/auth";
```

## [Client](./Client.md#client)

```typescript
const authClient = new AuthClient();
```

## [Authentication](./Function.md#basic-authentication)

```typescript
await authClient.login("BestUsername", "SuperSecretPassword");
```

```typescript
if (authClient.authenticationInfo.isMultifactor === true) {
    const verificationCode = 428793;

    await authClient.verify(verificationCode);
}
```

## Subject (PlayerUUID)

```typescript
const subject = authClient.getSubject();
```

## [Cookie](./Function.md#cookie)

```typescript
const authClient = await AuthClient.fromCookie(cookie);
```

## [Save](./Client.md#save)

```typescript
const authClient = AuthClient.fromJSON(_authClient.toJSON());

if (Date.now() >= authClient.getExpirationDate()) {
    await authClient.refresh();
}
```
