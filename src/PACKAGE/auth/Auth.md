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

**we recommend running this after creating *AuthClient***

```typescript
await AuthClient.refresh(isForce?);
```

## Cookie

you can save only SSID cookie for ~30 days.

```typescript
const AuthClient = await ValAuth.fromCookie(cookie.ssid);
```