# API

-----------

Something is can't use, so I did't insert it.

| Service       | Function     | ...Args           |
| ------------- | ------------ | ----------------- |
| **AccountV1** | ByRiotId     | gameName, tagLine |
|               | ByPuuid      | puuid             |
|               | ByGame       | puuid, game       |
| **ContentV1** | Contents     | locale            |
| **StatusV1**  | PlatformData |                   |

## Usage

```typescript
    const _data = await ApiClient.{Service}.{Function(...Args)}
```