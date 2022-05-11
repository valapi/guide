# Example

-----------

```typescript
import { Client } from '@valapi/riot-client';
```

## Client

```typescript
const ApiClient = new Client({
    ip: '127.0.0.1',
    path: 'C:/Users/Windows10/AppData/Local/Riot Games/Riot Client/Config/lockfile',
});

```

## Auth

```typescript
ApiClient.LockfileAuth();
```

## API

```typescript
const _data = await ApiClient.Chat.All_Chat_History();

console.log(_data.data);
```