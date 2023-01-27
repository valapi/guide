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
        platform?: {
            platformType: string;
            platformOS: string;
            platformOSVersion: string;
            platformChipset: string;
        };
    };

    /**
     * Request Config
     */
    axiosConfig?: AxiosRequestConfig;

    /**
     * Throw the Error?
     */
    throwOnError?: boolean;

    /**
     * Region
     */
    region?: string;
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
AuthClient.fromJSON(config, authClient.toJSON());
```
