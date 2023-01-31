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
const versions = await valorantApiCom.Versions.get();

console.log(versions.data);
```

```typescript
const mapUuid = "7eaecc1b-4337-bbf6-6ab9-04b8f06b3319"; /* Ascent */
const map = await valorantApiCom.Maps.getByUuid(mapUuid);

console.log(events.data);
```
