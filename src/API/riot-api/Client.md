# Introduced

---

```typescript
import { Client } from "@valapi/riot-api";
```

## Config

You Can Get Api Key From [developer.riotgames.com](https://developer.riotgames.com)

```typescript
interface Config {
    /**
     * API Key
     */
    apiKey: string;

    /**
     * Region
     */
    region: string;

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
