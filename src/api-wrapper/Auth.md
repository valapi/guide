# Authentication

-----------

## Login

First We Need To **Login** To `Valorant Account`

```typescript
await ApiClient.login('Username', 'Password');
```

*But We Have 2 Type Of Account*
 
## Multi-Factor

<details>
<summary>Example</summary>
<blockquote>

```typescript
const ApiClient = Client.fromJSON(config, old_ApiClient.toJSON());
await ApiClient.verify(123456);
```

</blockquote>
</details>

When The Account Have **Multifactor** You Can't Use Normal Method

After Login The **Verify Code** Will Send To Mail

```typescript
await ApiClient.verify(Number);
```

## Cookie

*Beta*

```typescript
await Client.fromCookie(config, old_ApiClient.toJSON());
```