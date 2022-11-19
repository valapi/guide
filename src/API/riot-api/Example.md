# Example

---

```typescript
import { Client } from "@valapi/riot-api";
```

## [Client](./Client.md#config)

```typescript
const ApiClient = new Client({
    apiKey: "LoooooongApiKey_123456789",
    region: "ap"
});
```

## [API](./API.md#usage)

```typescript
const data = await ApiClient.AccountV1.byRiotId("PRX f0rsakeN", "Huh");

console.log(data.data);
```
