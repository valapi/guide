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

    // When Token is expired, it will be refreshed.
    autoReconnect?: boolean;

    // When Cookie is expired, it will be refreshed.
    // * Not Support Multi-Factor Authentication.
    autoAuthentication?: {
        username: string,
        password: string,
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
ApiClient.toJSONAuth(); //more data (recommended for auth)
```

## Save --> Client

```typescript
Client.fromJSON(config, ApiClient.toJSON()); //you can use {.toJSONAuth} as a option
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