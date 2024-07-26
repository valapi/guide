# Introduced

---

```typescript
import { AuthClient } from "@valapi/auth";
```

## Config

```typescript
interface Config {
    /**
     * User
     */
    user?: AuthUserInfo;

    /**
     * User Agent
     */
    userAgent?: string;

    /**
     * Client Version
     */
    version?: string;

    /**
     * Client Platform
     */
    platform?: ClientPlatfrom;

    /**
     * Request Config
     */
    axiosConfig?: AxiosRequestConfig;

    /**
     * HTTP Agent Config
     */
    agentConfig?: AgentOptions & CookieAgentOptions;
}
```

## Client

```typescript
const auth = new Auth( config? );
```

# Save

---

## Client --> Save

```typescript
auth.toJSON();
```
