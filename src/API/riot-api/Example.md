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
const status = await riotApi.StatusV1.platformData();

console.log(status.data);
```

```typescript
const accountData = await riotApi.AccountV1.byRiotId("PRX f0rsakeN", "Huh");

console.log(accountData.data);
```
