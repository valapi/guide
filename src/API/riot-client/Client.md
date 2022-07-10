# Introduced

-----------

This API changes when **Riot Client** restart and is not the same on any devices.

```typescript
import { Client } from '@valapi/riot-client';
```

## Config

```typescript
interface Config {
    ip?: string;
    path?:string;
    username?: string;
    axiosConfig? : AxiosRequestConfig;
}
```

## Client

```typescript
const ApiClient = new Client( config? );
```

# Settings

-----------

| Setting  | Function    | ...Args  |
| -------- | ----------- | -------- |
| IP       | setIp       | ip       |
| Username | setUsername | username |
| Lockfile | setLockfile | name     |

## Usage

```javascript
    ApiClient.{Function(...Args)};
```