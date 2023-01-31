# Basic Authentication

---

## Login

First We Need To **Login** To `Valorant Account`

```typescript
await authClient.login("Username", "Password");
```

_But We Have 2 Type Of Account_

## Multi-Factor

When The Account Have **Multifactor** You Can't Use Normal Method

After Login The **Verify Code** Will Send To Mail

```typescript
await authClient.verify(SixDigitNumber);
```

# Advanced Authentication

---

## Reconnection

reconnection for getting a new token

**we recommend running this after importing _AuthClient_**

```typescript
await authClient.refresh();
```

## Cookie

you can save only SSID cookie for ~30 days.

```typescript
const cookie = (authClient.toJSON()).cookie.ssid;

const authClient = await AuthClient.fromCookie(cookie);
```
