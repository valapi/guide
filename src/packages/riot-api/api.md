# API

---

| Service       | Function                   | Arguments                 |
| ------------- | -------------------------- | ------------------------- |
| **AccountV1** | byPuuid                    | puuid                     |
|               | byRiotId                   | gameName, tagLine         |
|               | activeShardsByGameAndPuuid | puuid, game?              |
|               | byAccessToken              | authorization             |
| **ContentV1** | contents                   | locale?                   |
| **MatchV1**   | byMatchId                  | matchId                   |
|               | listByPuuid                | puuid                     |
|               | recentByQueue              | queueId                   |
| **RankedV1**  | leaderboardsByAct          | actId, size?, startIndex? |
| **StatusV1**  | platformData               |                           |

## Usage

```typescript
const data = await riotApi.Service.Function(...Arguments);
```
