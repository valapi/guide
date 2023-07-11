# Basic Authentication

---

## Login

First, We need to log in to an account

```typescript
await authClient.login("Username", "Password");
```

## Multi-Factor

After login, the **Verification Code** will be sent to your mail if a multi-factor is enabled

```typescript
await authClient.verify(SixDigitNumber);
```

# Advanced Authentication

---

## Reconnection

Reconnection for getting a new token

**we recommend running this after importing _AuthClient_ or every 1 hour**

```typescript
await authClient.refresh();
```

## Cookie

You can save only cookies for ~30 days

```typescript
const cookie = authClient.cookie;

const authClient = await AuthClient.fromCookie(cookie);
```
