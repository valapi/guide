# Introduced

---

```typescript
import { Client } from "@valapi/valorant-api.com";
```

## Config

```typescript
interface Config {
    /**
     * Language
     */
    language?: string;

    /**
     * Request Config
     */
    axiosConfig?: AxiosRequestConfig;

    /**
     * Throw the Error?
     */
    throwOnError?: boolean;
}
```

## Client

```typescript
const ApiClient = new Client( config? );
```
