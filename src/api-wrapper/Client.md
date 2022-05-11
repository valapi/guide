# Introduced

-----------

```typescript
import { Client } from '@valapi/api-wrapper';
```

# Config

-----------

```typescript
interface Config {
    userAgent?: string;
    region?: string;
    client?: {
        version?: string;
        platform?: {
            "platformType": string;
            "platformOS": string;
            "platformOSVersion": string;
            "platformChipset": string;
        };
    };
    timeout?: number;
}
```

# Authentication

-----------

Create an **API Client**

```typescript
const ApiClient = new Client(config);
```

# Save

-----------

## Client --> Save

```typescript
ApiClient.toJSON();
```

## Save --> Client

```typescript
Client.fromJSON(config, ApiClient.toJSON());
```

# Settings

-----------

| Setting         | Function                             |
| --------------- | ------------------------------------ |
| Region          | setRegion *(region)*                 |
| Client Version  | setClientVersion *(clientVersion)*   |
| Client Platfrom | setClientPlatfrom *(clientPlatfrom)* |
| Cookie          | setClientPlatfrom *(cookie)*         |

```javascript
    ApiClient.{Function}
```