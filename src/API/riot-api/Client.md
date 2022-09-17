# Introduced

-----------

```typescript
import { Client } from '@valapi/riot-api';
```

## Config

```typescript
interface Config {
    /**
     * API Key
     */
    apiKey: string;

    /**
     * Region
     */
    region: string;

    /**
     * Expire time
     * The time in milliseconds that data will be refreshed.
     */
    expiresIn?: number;

    /**
     * Request Config
     * Config for RequestClient (Axios)
     */
    axiosConfig?: AxiosRequestConfig;

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

You Can Get Api Key From [developer.riotgames.com](https://developer.riotgames.com/)

# Settings

-----------

| Set     | Function  | ...Args |
| ------- | --------- | ------- |
| API Key | setApiKey | apiKey  |
| Region  | setRegion | region  |

## Usage

```javascript
    ApiClient.{Function(...Args)};
```