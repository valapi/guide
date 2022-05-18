# Introduced

-----------

```typescript
import { Client } from '@valapi/riot-api';
```

## Config

```typescript
interface Config {
    apiKey: string;
    region: string;
    axiosConfig?: AxiosRequestConfig;
}
```

## Client

```typescript
const ApiClient = new Client(config);
```

You Can Get Api Key From [developer.riotgames.com](https://developer.riotgames.com/)

# Settings

-----------

| Setting | Function  | ...Args |
| ------- | --------- | ------- |
| API Key | setApiKey | apiKey  |
| Region  | setRegion | region  |

## Usage

```javascript
    ApiClient.{Function(...Args)};
```