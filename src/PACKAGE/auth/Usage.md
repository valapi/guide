# Usage

---

```typescript
import { Client } from "@valapi/auth";
```

## [Client](./Client.md#client)

```typescript
const AuthClient = new Client();
```

## [Auth](./Auth.md#basic-authentication)

```typescript
await AuthClient.login("BestUsername", "SuperSecretPassword");
```

```typescript
if (AuthClient.isMultifactorAccount === true) {
    await AuthClient.verify(428793 /* <--- Verification Code */);
}
```

## Subject (PlayerUUID)

```typescript
const subject = AuthClient.getSubject();
```
