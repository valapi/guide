# Example

---

```typescript
import { AuthClient } from "@valapi/auth";
```

## [Client](./client.md)

```typescript
const auth = new Auth();
```

## [Authentication](./function.md)

```typescript
await auth.login("BestUsername", "SuperSecretPassword");
```

## Subject (PlayerUUID)

```typescript
const subject = auth.subject;
```

## [Cookie](./function.md)

```typescript
await auth.reauthorize();
```

## [Save](./client.md)

```typescript
const auth = new Auth({ user: oldAuth.toJSON() });

if (new Date() >= auth.expirationDate) {
    await auth.reauthorize();
}
```
