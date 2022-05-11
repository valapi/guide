# Introduced

-----------

This API changes when **Riot Client** restart and is not the same on any devices.

```typescript
import { Client } from '@valapi/riot-client';
```

# Config

-----------

```typescript
interface Config {
    ip?: string;
    lockfile?: {
        name: string;
        pid: number;
        port: number;
        password: string;
        protocol: string;
    };
    path?:string;
    username?: string;
    timeout?: number;
}
```

# Authentication

-----------

Create an **API Client**

```typescript
const ApiClient = new Client(config);
```

# Settings

-----------

| Setting  | Function                         |
| -------- | -------------------------------- |
| IP       | setIp *(ip)*                     |
| Username | setUsername *(username)*         |
| Lockfile | setLockfileName *(name)*         |
|          | setLockfilePid *(pid)*           |
|          | setLockfilePort *(port)*         |
|          | setLockfilePassword *(password)* |
|          | setLockfileProtocol *(protocol)* |

## Usage

```javascript
    ApiClient.{Function}
```