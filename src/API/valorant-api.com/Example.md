# Example

---

```typescript
import { ValorantApiCom } from "@valapi/valorant-api.com";
```

## [Client](./Client.md#config)

```typescript
const valorantApiCom = new ValorantApiCom({
    language: "en-US"
});
```

## [API](./API.md#usage)

```typescript
const data = await valorantApiCom.Events.get();

console.log(data.data);
```
