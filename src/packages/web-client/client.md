# Introduced

---

```typescript
import { WebClient } from "@valapi/web-client";
```

## Config

```typescript
interface Config {
    /**
     * Authenticated User
     */
    user: AuthUserInfo;

    /**
     * Account Region
     */
    region?: Region.ID;
}
```

## Client

```typescript
const client = new WebClient(config);
```
