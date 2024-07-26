# Example

---

```typescript
import { WebClient } from "@valapi/web-client";
```

## [Client](./client.md)

```typescript
const client = new WebClient({
    user: auth.toJSON()
});
```

## [API](./api.md)

```typescript
const userInfo = await client.getUserInfo();

console.log(userInfo.data);
```

```typescript
const mapId = "match-id-1234567890";
const matchDetails = await client.Match.fetchMatchDetails(mapId);

console.log(matchDetails.data);
```

```typescript
const wallet = await client.Store.getWallet(client.subject);

console.log(wallet.data);
```
