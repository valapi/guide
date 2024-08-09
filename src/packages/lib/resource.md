# Resources

---

| Resource          | Method   |
| ----------------- | -------- |
| CrosshairColor    | fromName |
|                   | fromID   |
| CrosshairHexColor | fromName |
|                   | fromHex  |
| ItemTypeId        | fromName |
|                   | fromID   |
| Locale            | fromName |
|                   | fromID   |
| QueueId           | fromName |
|                   | fromID   |
| Region            | fromName |
|                   | fromID   |

## Usage

---

```typescript
import { [Resource] } from "@valapi/lib";
```

```typescript
[Resource].fromName("Name"); // change name to identify
```

```typescript
[Resource].fromID("1id3"); // change identify to name
```