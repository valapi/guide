# Introduced

-----------

```typescript
import { Client } from '@valapi/auth';
```

## Config

```typescript
interface Config {
    /**
     * Client Config
     */
    client?: {
        version?: string,
        platform?: {
            "platformType": string,
            "platformOS": string,
            "platformOSVersion": string,
            "platformChipset": string,
        },
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
        cookie: number,
        token?: number,
    };
}
```

## Client

```typescript
const AuthClient = new Client( config? );
```

# Save

-----------

## Client --> Save

```typescript
AuthClient.toJSON();
```

## Save --> Client

```typescript
Client.fromJSON(config, AuthClient.toJSON());
```