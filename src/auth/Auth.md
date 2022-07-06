# Basic Authentication

-----------

## Login

First We Need To **Login** To `Valorant Account`

```typescript
await AuthClient.login('Username', 'Password');
```

*But We Have 2 Type Of Account*
 
## Multi-Factor

When The Account Have **Multifactor** You Can't Use Normal Method

After Login The **Verify Code** Will Send To Mail

```typescript
await AuthClient.verify(SixDigitNumber);
```

# Advanced Authentication

-----------

## Reconnection

its will reconnection if the token is expired

```typescript
await AuthClient.reload(isForce?);
```

## Cookie

```typescript
const AuthClient = await ValRso.fromCookie(cookie);
```