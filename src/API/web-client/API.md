# API

-----------

<https://github.com/techchrism/valorant-api-docs>

| Service         | Function                   | ...Args                                       |
| --------------- | -------------------------- | --------------------------------------------- |
| **Contract**    | DefinitionsFetch           |                                               |
|                 | FetchActiveStory           | puuid                                         |
|                 | Fetch                      | puuid                                         |
|                 | Active                     | puuid, contractId                             |
| **CurrentGame** | FetchAllChatMUCToken       | matchId                                       |
|                 | FetchMatch                 | matchId                                       |
|                 | FetchMatchLoadouts         | matchId                                       |
|                 | FetchPlayer                | puuid                                         |
|                 | FetchTeamChatMUCToken      | matchId                                       |
|                 | DisassociatePlayer         | puuid, matchId                                |
| **Party**       | RemovePlayer               | puuid                                         |
|                 | FetchCustomGameConfigs     |                                               |
|                 | FetchMUCToken              | partyId                                       |
|                 | FetchParty                 | partyId                                       |
|                 | FetchPlayer                | puuid                                         |
|                 | FetchVoiceToken            | partyId                                       |
|                 | ChangeQueue                | partyId, queue                                |
|                 | DeclineRequest             | partyId, requestId                            |
|                 | EnterMatchmakingQueue      | partyId                                       |
|                 | InviteToPartyByDisplayName | partyId, gameName, tagLine                    |
|                 | LeaveMatchmakingQueue      | partyId                                       |
|                 | RefreshCompetitiveTier     | puuid, partyId                                |
|                 | RefreshPings               | puuid, partyId                                |
|                 | RefreshPlayerIdentity      | puuid, partyId                                |
|                 | SetAccessibility           | partyId, accessibility                        |
|                 | SetCustomGameSettings      | partyId, settings                             |
|                 | SetMemberReady             | partyId, puuid, isReady                       |
|                 | StartCustomGame            | partyId                                       |
|                 | LeaveParty                 | puuid, partyId                                |
|                 | AutoBalance                | partyId                                       |
|                 | ChangeTeamInCustomGame     | partyId, team, puuid                          |
|                 | StartSoloExperience        | partyId                                       |
|                 | TransferOwner              | puuid, partyId                                |
| **PreGame**     | FetchChatToken             | matchId                                       |
|                 | FetchVoiceToken            | matchId                                       |
|                 | GetMatch                   | matchId                                       |
|                 | GetMatchLoadouts           | matchId                                       |
|                 | GetPlayer                  | puuid                                         |
|                 | LockCharacter              | matchId, agentId                              |
|                 | QuitMatch                  | matchId                                       |
|                 | SelectCharacter            | matchId, agentId                              |
| **Session**     | Get                        | puuid                                         |
|                 | ReConnect                  | puuid                                         |
| **Store**       | GetEntitlements            | puuid, itemTypeId                             |
|                 | GetOffers                  |                                               |
|                 | GetStorefront              | puuid                                         |
|                 | GetWallet                  | puuid                                         |
|                 | RevealNightMarketOffers    | puuid                                         |
| **App**         | FetchContent               |                                               |
|                 | FetchConfig                |                                               |
| **Match**       | FetchMatchDetails          | matchId                                       |
|                 | FetchMatchHistory          | puuid, queueId?, startIndex?, endIndex?       |
| **MMR**         | FetchCompetitiveUpdates    | puuid, queueId?, startIndex?, endIndex?       |
|                 | FetchLeaderboard           | seasonId, startIndex?, size?, serachUsername? |
|                 | FetchPlayer                | puuid                                         |
|                 | HideActRankBadge           | puuid                                         |
| **Player**      | GetUsername                | puuid                                         |
|                 | GetUserInfo                |                                               |
|                 | AccountXP                  | puuid                                         |
|                 | Loadout                    | puuid                                         |
|                 | LoadoutUpdate              | puuid                                         |
|                 | FetchPlayerRestrictions    |                                               |
|                 | MassRewards                | puuid                                         |

## Usage

```typescript
    const _data = await ApiClient.{Service}.{Function(...Args)};
```