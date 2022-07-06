# Introduced

-----------

```typescript
import { Client } from '@valapi/riot-api';
```

## Config

```typescript
interface Config {
    language?: string;
    axiosConfig?: AxiosRequestConfig;
}
```

## Client

```typescript
const ApiClient = new Client(config?);
```

# Settings

-----------

| Setting  | Function    | ...Args  |
| -------- | ----------- | -------- |
| Language | setLanguage | language |

## Usage

```javascript
    ApiClient.{Function(...Args)};
```