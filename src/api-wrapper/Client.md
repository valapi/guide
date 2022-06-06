# Introduced

-----------

```typescript
import { Client } from '@valapi/api-wrapper';
```

## Config

```typescript
interface Config {
    // UserAgent use when authentication
    userAgent?: string;

    // Region of the Account
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

    // No throw error if the authentication is failed.
    forceAuth?: boolean;

    // Config for RequestClient (Axios)
    axiosConfig?: AxiosRequestConfig;

    // The time in milliseconds that data will be refreshed.
    expiresIn?: {
        cookie: number,
        token?: number,
    };

    // When Cookie is expired, it will be refreshed.
    selfAuthentication?: {
        username: string | Function,
        password: string | Function,
        verifyCode?: string | number | Function,
    };
}
```

## Client

```typescript
const ApiClient = new Client(config);
```

# Save

-----------

## Client --> Save

```typescript
ApiClient.toJSON();
```

```typescript
ApiClient.toJSONAuth(); // recommended for authentication
```

## Save --> Client

```typescript
Client.fromJSON(config, ApiClient.toJSON());
```

```typescript
Client.fromJSONAuth(config, ApiClient.toJSONAuth());
```

# Settings

-----------

| Setting         | Function          | ...Args        |
| --------------- | ----------------- | -------------- |
| Region          | setRegion         | region         |
| Client Version  | setClientVersion  | clientVersion  |
| Client Platfrom | setClientPlatfrom | clientPlatfrom |
| Cookie          | setClientPlatfrom | cookie         |

## Usage

```javascript
    ApiClient.{Function(...Args)};
```