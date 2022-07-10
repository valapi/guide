# Basic Authentication

-----------

## Login

First We Need To **Login** To `Valorant Account`

```typescript
await ApiClient.login('Username', 'Password');
```

*But We Have 2 Type Of Account*
 
## Multi-Factor

When The Account Have **Multifactor** You Can't Use Normal Method

After Login The **Verify Code** Will Send To Mail

```typescript
await ApiClient.verify(Number);
```

# Advanced Authentication

-----------

*Beta*

## Cookie

```typescript
await ApiClient.fromCookie(cookie?);
```

## Reconnection

its will reconnection if the token or cookie is expired

```typescript
await ApiClient.reconnect(isForce?); // isForce = only reconnect token;
```