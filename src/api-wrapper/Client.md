# Introduced

-----------

```typescript
import { Client } from '@valapi/api-wrapper';
```

## Config

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
    axiosConfig?: AxiosRequestConfig,
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