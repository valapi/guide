# Introduced

-----------

```typescript
import { Client } from '@valapi/riot-api';
```

## Config

```typescript
interface Config {
    /**
     * Language
     */
    language?: string;

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

# Settings

-----------

| Set      | Function    | ...Args  |
| -------- | ----------- | -------- |
| Language | setLanguage | language |

## Usage

```javascript
    ApiClient.{Function(...Args)};
```