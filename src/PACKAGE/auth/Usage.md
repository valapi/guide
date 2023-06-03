# Usage

---

```typescript
import { AuthClient } from "@valapi/auth";
```

## [Client](./Client.md#client)

```typescript
const authClient = new AuthClient();
```

## [Auth](./Auth.md#basic-authentication)

```typescript
await authClient.login("BestUsername", "SuperSecretPassword");
```

```typescript
if (authClient.isMultifactorAccount === true) {
    await authClient.verify(428793 /* <--- Verification Code */);
}
```

## Subject (PlayerUUID)

```typescript
const subject = authClient.getSubject();
```

## [Cookie](./Auth.md#cookie)

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
