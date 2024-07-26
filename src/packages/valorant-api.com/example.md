# Example

---

```typescript
import { ValorantApiCom } from "@valapi/valorant-api.com";
```

## [Client](./client.md)

```typescript
const client = new ValorantApiCom({
    language: "en-US"
});
```

## [API](./api.md)

```typescript
const versions = await client.Versions.get();

console.log(versions.data);
```

```typescript
const mapUuid = "7eaecc1b-4337-bbf6-6ab9-04b8f06b3319"; /* Ascent */
const map = await client.Maps.getByUuid(mapUuid);

console.log(map.data);
```
