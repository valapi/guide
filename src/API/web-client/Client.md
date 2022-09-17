# Introduced

-----------

```typescript
import { Client } from '@valapi/web-client';
```

## Config

```typescript
interface Config {
    /**
     * Region
     */
    region?: string;

    /**
     * Client Config
     */
    client?: {
        version?: string;
        platform?: {
            "platformType": string;
            "platformOS": string;
            "platformOSVersion": string;
            "platformChipset": string;
        };
    };

    /**
     * Request Config
     * Config for RequestClient (Axios)
     */
    axiosConfig?: AxiosRequestConfig;

    /**
     * Expire time
     * The time in milliseconds that data will be refreshed.
     */
    expiresIn?: {
        cookie: number;
        token?: number;
    };

    /**
     * Throw the Error?
     */
    throwOnError?: boolean;
}
```

## Client

```typescript
const ApiClient = new Client( config? );
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

| Set             | Function          | ...Args        |
| --------------- | ----------------- | -------------- |
| Region          | setRegion         | region         |
| Client Version  | setClientVersion  | clientVersion  |
| Client Platfrom | setClientPlatfrom | clientPlatfrom |

## Usage

```javascript
    ApiClient.{Function(...Args)};
```