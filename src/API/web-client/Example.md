# Example

---

**this client is based on an [Authentication Client](../../PACKAGE/auth/Usage.md)**

```typescript
import { WebClient } from "@valapi/web-client";
```

## [API](./API.md#usage)

```typescript
const data = await webClient.PreGame.getMatch("MATCH-ID-1234567890");

console.log(data.data);
```
