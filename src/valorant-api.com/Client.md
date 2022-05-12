# Introduced

-----------

```typescript
import { Client } from '@valapi/riot-api';
```

# Config

-----------

```typescript
interface Config {
    language?: string; //can use 'all' language but not supported yet
    axiosConfig?: AxiosRequestConfig;
}
```

# Authentication

-----------

Create an **API Client**

```typescript
const ApiClient = new Client(config);
```

# Settings

-----------

| Setting  | Function    | ...Args  |
| -------- | ----------- | -------- |
| Language | setLanguage | language |

## Usage

```javascript
    ApiClient.{Function(...Args)}
```