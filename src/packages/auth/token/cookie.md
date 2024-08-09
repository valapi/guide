# Cookie Authorization

---

You can save only cookies for ~30 days

```typescript
import { AuthInstance } from "@valapi/auth";
```

```typescript
const instance = new AuthInstance({ cookie: serializeCookie });

const auth = new Auth({ user: instance.toJSON() });
```

I recommend running this every time you deserialize

```typescript
// new Date() >= auth.expirationDate

if (!auth.isAuthenticated) {
    await auth.reauthorize();
}
```

---

ref.

- [AuthInstance](https://valapi.github.io/docs/classes/auth.AuthInstance.html#cookie)
- [serializeCookie](../client.md#serialize)
- [Auth#isAuthenticated](https://valapi.github.io/docs/classes/auth.AuthInstance.html#isAuthenticated)