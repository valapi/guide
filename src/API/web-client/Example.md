# Example

---

**this client is based on an [Authentication Client](../../PACKAGE/auth/Usage.md)**

```typescript
import { WebClient } from "@valapi/web-client";
```

## [API](./API.md#usage)

```typescript
const userInfo = await webClient.getUserInfo();

console.log(userInfo.data);
```

```typescript
const matchDetails = await webClient.Match.fetchMatchDetails("match-id-1234567890");

console.log(matchDetails.data);
```

```typescript
const wallet = await webClient.Store.getWallet(subject);

console.log(wallet.data);
```