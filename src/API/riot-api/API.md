# API

-----------

| Service       | Function                   | ...Args                   |
| ------------- | -------------------------- | ------------------------- |
| **AccountV1** | ByPuuid                    | puuid                     |
|               | ByRiotId                   | gameName, tagLine         |
|               | ActiveShardsByGameAndPuuid | puuid, game?              |
| **ContentV1** | Contents                   | locale?                   |
| **MatchV1**   | ByMatchId                  | matchId                   |
|               | ListByPuuid                | puuid                     |
|               | RecentByQueue              | queueId                   |
| **RankedV1**  | LeaderboardsByAct          | actId, size?, startIndex? |
| **StatusV1**  | PlatformData               |                           |

## Usage

```typescript
    const _data = await ApiClient.{Service}.{Function(...Args)};
```