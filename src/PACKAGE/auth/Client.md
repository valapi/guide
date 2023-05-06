# Introduced

---

```typescript
import { AuthClient } from "@valapi/auth";
```

## Config

```typescript
interface Config {
    /**
     * Client Config
     */
    client?: {
        /**
         * Client Version
         */
        version?: string;
        /**
         * Client Platform
         */
        platform?: AuthCore.ClientPlatfrom;
    };

    /**
     * Request Config
     */
    axiosConfig?: CreateAxiosDefaults;

    /**
     * Region
     */
    region?: Region.Identify;
}
```

## Client

```typescript
const authClient = new AuthClient( config? );
```

# Save

---

## Client --> Save

```typescript
authClient.toJSON();
```

## Save --> Client

```typescript
AuthClient.fromJSON( authClient.toJSON(), config? );
```
