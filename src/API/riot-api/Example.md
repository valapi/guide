# Example

---

```typescript
import { RiotApi } from "@valapi/riot-api";
```

## [Client](./Client.md#config)

```typescript
const riotApi = new RiotApi({
    apiKey: "LoooooongApiKey_123456789",
    region: "ap"
});
```

## [API](./API.md#usage)

```typescript
const data = await riotApi.AccountV1.byRiotId("PRX f0rsakeN", "Huh");

console.log(data.data);
```
