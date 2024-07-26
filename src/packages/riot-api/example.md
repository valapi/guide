# Example

---

```typescript
import { RiotApi } from "@valapi/riot-api";
```

## [Client](./client.md)

```typescript
const client = new RiotApi({
    apiKey: "LoooooongApiKey_123456789",
    region: "ap"
});
```

## [API](./api.md)

```typescript
const status = await client.StatusV1.platformData();

console.log(status.data);
```

```typescript
const accountData = await client.AccountV1.byRiotId("PRX f0rsakeN", "Huh");

console.log(accountData.data);
```
