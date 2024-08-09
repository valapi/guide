# Identity Authorization

---

Once these steps are finished, the authorization should be finished as well

## Login credentials

```typescript
await auth.login({
    username: "BestUsername",
    password: "SuperSecretPassword",
    captcha: captchaResponse
});
```

## Multi-factor authentication

```typescript
if (auth.isMultifactor) {
    const loginCode = 428793;

    await auth.multifactor(loginCode);
}
```

---

ref.

- [auth](../client.md#constructor)
- [captchaResponse](./captcha.md)
- [Auth#isMultifactor](https://valapi.github.io/docs/classes/auth.AuthInstance.html#isMultifactor)