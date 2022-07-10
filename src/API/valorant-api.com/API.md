# API

-----------

All API base on [dash.valorant-api.com](https://dash.valorant-api.com/)

| Service              | Function                   | ...Args             |
| -------------------- | -------------------------- | ------------------- |
| **Agent**            | get                        | isPlayableCharacter |
|                      | getByUuid                  | uuid                |
| **Buddies**          | get                        |                     |
|                      | getLevels                  |                     |
|                      | getByUuid                  | uuid                |
|                      | getLevelByUuid             | uuid                |
| **Bundles**          | get                        |                     |
|                      | getByUuid                  | uuid                |
| **Bundles**          | get                        |                     |
|                      | getByUuid                  | uuid                |
| **Ceremonies**       | get                        |                     |
|                      | getByUuid                  | uuid                |
| **CompetitiveTiers** | get                        |                     |
|                      | getByUuid                  | uuid                |
| **ContentTiers**     | get                        |                     |
|                      | getByUuid                  | uuid                |
| **Contracts**        | get                        |                     |
|                      | getByUuid                  | uuid                |
| **Currencies**       | get                        |                     |
|                      | getByUuid                  | uuid                |
| **Events**           | get                        |                     |
|                      | getByUuid                  | uuid                |
| **Gamemodes**        | get                        |                     |
|                      | getEquippables             |                     |
|                      | getByUuid                  | uuid                |
|                      | getEquippableByUuid        | uuid                |
| **Gear**             | get                        |                     |
|                      | getByUuid                  | uuid                |
| **Maps**             | get                        |                     |
|                      | getByUuid                  | uuid                |
| **PlayerCards**      | get                        |                     |
|                      | getByUuid                  | uuid                |
| **PlayerTitles**     | get                        |                     |
|                      | getByUuid                  | uuid                |
| **Seasons**          | get                        |                     |
|                      | getCompetitiveSeasons      |                     |
|                      | getByUuid                  | uuid                |
|                      | getCompetitiveSeasonByUuid | uuid                |
| **Sprays**           | get                        |                     |
|                      | getLevels                  |                     |
|                      | getByUuid                  | uuid                |
|                      | getLevelByUuid             | uuid                |
| **Themes**           | get                        |                     |
|                      | getByUuid                  | uuid                |
| **Versions**         | get                        |                     |
| **Weapons**          | get                        |                     |
|                      | getSkins                   |                     |
|                      | getSkinChromas             |                     |
|                      | getSkinLevels              |                     |
|                      | getByUuid                  | uuid                |
|                      | getSkinByUuid              | uuid                |
|                      | getSkinChromaByUuid        | uuid                |
|                      | getSkinLevelByUuid         | uuid                |

## Usage

```typescript
    const _data = await ApiClient.{Service}.{Function(...Args)};
```