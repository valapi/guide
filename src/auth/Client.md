# Introduced

-----------

```typescript
import { ValRso } from '@valapi/auth';
```

## Config

```typescript
interface Config {
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
const AuthClient = new ValRso(config?);
```

# Save

-----------

## Client --> Save

```typescript
AuthClient.toJSON();
```

## Save --> Client

```typescript
ValRso.fromJSON(config, AuthClient.toJSON());
```