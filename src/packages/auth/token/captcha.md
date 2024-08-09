# CAPTCHAs

---

> This is an example of many ways to get a captcha response

```typescript
const hCaptcha = await auth.captcha();
```

```typescript
interface hCaptcha {
    sitekey: string;
    rqdata: string;
}
```

## Express

Setup an express server

```bash
npm install express
```

```typescript
import * as express from "express";

const port = 8880;
const app = express();

app.get("/", (req, res) => {
    res.sendFile("index.html");
});

app.get("/captcha", (req, res) => {
    res.send(hCaptcha);
});

app.get("/verify/:token", async (req, res) => {
    res.sendStatus(200);

    app.set("captchaResponse", req.params.token);
});

app.listen(port);
```

```html
<html>

<head>
  <script src="https://cdn.jsdelivr.net/npm/@hcaptcha/vanilla-hcaptcha" async defer></script>
</head>

<body>
  <h-captcha id="signupCaptcha" auto-render="false"></h-captcha>
</body>

<script>
  window.onload = async () => {
    const captcha = document.getElementById('signupCaptcha');

    const response = await fetch("/captcha");
    const data = await response.json();

    captcha.render({ "sitekey": data.sitekey });
    captcha.setData(data.rqdata);

    captcha.addEventListener('verified', async event => {
      await fetch(`/verify/${event.token}`);
    });
  };
</script>

</html>
```

get a captcha response

```typescript
const captchaResponse = app.set("captchaResponse");
```

## CAPTCHA Solver

> npmjs/valapi will not assist and be relevant in any legal actions that happen when using Captcha Solver, so **use it at your own risk**

```typescript
const captchaResponse = await CaptchaSolver({
    type: "HCaptchaTaskProxyLess",
    url: "https://auth.riotgames.com",
    sitekey: hCaptcha.sitekey,
    rqdata: hCaptcha.rqdata,
});
```

---

ref.

- [auth](../client.md#constructor)
- [express](https://www.npmjs.com/package/express)
- [@hcaptcha/vanilla-hcaptcha](https://www.npmjs.com/package/@hcaptcha/vanilla-hcaptcha)