# Introduced

---

```typescript
import { ValorantApiCom } from "@valapi/valorant-api.com";
```

## Config

```typescript
interface Config {
    /**
     * Language
     */
    language?: ValorantApiCom.Language;

    /**
     * Request Config
     */
    axiosConfig?: CreateAxiosDefaults;

    /**
     * Response Option
     */
    responseOptions?: {
        /**
         * Delete properties that have a `null` value
         */
        ignore_null?: boolean;
    };
}
```

## Client

```typescript
const client = new ValorantApiCom( config? );
```
