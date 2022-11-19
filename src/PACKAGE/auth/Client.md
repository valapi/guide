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
        /**
         * Client Version
         */
        version?: string,
        
        /**
         * Client Platform
         */
        platform?: {
            "platformType": string,
            "platformOS": string,
            "platformOSVersion": string,
            "platformChipset": string,
        },
    };

    /**
     * Request Config
     */
    axiosConfig?: AxiosRequestConfig;

    /**
     * Throw the Error?
     */
    throwOnError?: boolean;

    /**
     * Region
     */
    region?: string;
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