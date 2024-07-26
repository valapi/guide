# Basic Authentication

---

## Login

```typescript
await auth.login("Username", "Password");
```

# Advanced Authentication

---

## Reconnection

Reconnection for getting a new token

**we recommend running this after importing _Auth_ or every 1 hour**

```typescript
await auth.reauthorize();
```

## Cookie

You can save only cookies for ~30 days

```typescript
const instance = new AuthInstance({ cookie: oldAuth.cookie.serializeSync() });

const auth = new Auth({ user: instance.toJSON() });

if (new Date() >= auth.expirationDate) {
    await auth.reauthorize();
}
```
