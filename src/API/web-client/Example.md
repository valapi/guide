# Example

---

```typescript
import { WebClient } from "@valapi/web-client";
```

## [API](./API.md#usage)

```typescript
const userInfo = await webClient.getUserInfo();

console.log(userInfo.data);
```

```typescript
const mapId = "match-id-1234567890";
const matchDetails = await webClient.Match.fetchMatchDetails(mapId);

console.log(matchDetails.data);
```

```typescript
const wallet = await webClient.Store.getWallet(subject);

console.log(wallet.data);
```
