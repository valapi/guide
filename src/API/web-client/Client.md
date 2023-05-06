# Introduced

> This client is based on [@valapi/auth/AuthClient](../../PACKAGE/auth/Client.md)

---

```typescript
import { WebClient } from "@valapi/web-client";
```

## Client

```typescript
const webClient = new WebClient( config? );
```

# Save ( User )

---

Save only important things

## Client --> Save

```typescript
webClient.toUserJSON();
```

## Save --> Client

```typescript
WebClient.fromUserJSON( webClient.toUserJSON(), config? );
```
