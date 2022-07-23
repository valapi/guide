# Introduced

-----------

```typescript
import { Client } from '@valapi/web-client';
```

## Config

```typescript
interface Config {
    // Region
    region?: string;

    // Client Settings
    client?: {
        version?: string,
        platform?: {
            "platformType": string,
            "platformOS": string,
            "platformOSVersion": string,
            "platformChipset": string,
        },
    };

    // Config for RequestClient (Axios)
    axiosConfig?: AxiosRequestConfig;

    // The time in milliseconds that data will be refreshed.
    expiresIn?: {
        cookie: number,
        token?: number,
    };
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