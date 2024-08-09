# Introduced

---

```typescript
import { RiotApi } from "@valapi/riot-api";
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
    region: Region.Identify;

    /**
     * Request Config
     */
    axiosConfig?: CreateAxiosDefaults;
}
```

## Client

```typescript
const client = new RiotApi([config]);
```
