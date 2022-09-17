# API

-----------

<https://github.com/techchrism/valorant-api-docs>

| Service         | Function                   | ...Args                                       |
| --------------- | -------------------------- | --------------------------------------------- |
| **Contract**    | definitionsFetch           |                                               |
|                 | fetchActiveStory           | puuid                                         |
|                 | fetch                      | puuid                                         |
|                 | active                     | puuid, contractId                             |
| **CurrentGame** | fetchAllChatMUCToken       | matchId                                       |
|                 | fetchMatch                 | matchId                                       |
|                 | fetchMatchLoadouts         | matchId                                       |
|                 | fetchPlayer                | puuid                                         |
|                 | fetchTeamChatMUCToken      | matchId                                       |
|                 | disassociatePlayer         | puuid, matchId                                |
| **Party**       | removePlayer               | puuid                                         |
|                 | fetchCustomGameConfigs     |                                               |
|                 | fetchMUCToken              | partyId                                       |
|                 | fetchParty                 | partyId                                       |
|                 | fetchPlayer                | puuid                                         |
|                 | fetchVoiceToken            | partyId                                       |
|                 | changeQueue                | partyId, queue                                |
|                 | declineRequest             | partyId, requestId                            |
|                 | enterMatchmakingQueue      | partyId                                       |
|                 | inviteToPartyByDisplayName | partyId, gameName, tagLine                    |
|                 | leaveMatchmakingQueue      | partyId                                       |
|                 | refreshCompetitiveTier     | puuid, partyId                                |
|                 | refreshPings               | puuid, partyId                                |
|                 | refreshPlayerIdentity      | puuid, partyId                                |
|                 | setAccessibility           | partyId, accessibility                        |
|                 | setCustomGameSettings      | partyId, settings                             |
|                 | setMemberReady             | partyId, puuid, isReady                       |
|                 | startCustomGame            | partyId                                       |
|                 | leaveParty                 | puuid, partyId                                |
|                 | autoBalance                | partyId                                       |
|                 | changeTeamInCustomGame     | partyId, team, puuid                          |
|                 | startSoloExperience        | partyId                                       |
|                 | transferOwner              | puuid, partyId                                |
| **PreGame**     | getchChatToken             | matchId                                       |
|                 | fetchVoiceToken            | matchId                                       |
|                 | getMatch                   | matchId                                       |
|                 | getMatchLoadouts           | matchId                                       |
|                 | getPlayer                  | puuid                                         |
|                 | lockCharacter              | matchId, agentId                              |
|                 | quitMatch                  | matchId                                       |
|                 | selectCharacter            | matchId, agentId                              |
| **Session**     | get                        | puuid                                         |
|                 | reConnect                  | puuid                                         |
| **Store**       | getEntitlements            | puuid, itemTypeId                             |
|                 | getOffers                  |                                               |
|                 | getStorefront              | puuid                                         |
|                 | getWallet                  | puuid                                         |
|                 | revealNightMarketOffers    | puuid                                         |
| **App**         | fetchContent               |                                               |
|                 | fetchConfig                |                                               |
| **Match**       | fetchMatchDetails          | matchId                                       |
|                 | fetchMatchHistory          | puuid, queueId?, startIndex?, endIndex?       |
| **MMR**         | fetchCompetitiveUpdates    | puuid, queueId?, startIndex?, endIndex?       |
|                 | fetchLeaderboard           | seasonId, startIndex?, size?, serachUsername? |
|                 | fetchPlayer                | puuid                                         |
|                 | hideActRankBadge           | puuid                                         |
| **Player**      | getUsername                | puuid                                         |
|                 | getUserInfo                |                                               |
|                 | accountXP                  | puuid                                         |
|                 | loadout                    | puuid                                         |
|                 | loadoutUpdate              | puuid                                         |
|                 | fetchPlayerRestrictions    |                                               |
|                 | massRewards                | puuid                                         |

## Usage

```typescript
    const _data = await ApiClient.{Service}.{Function(...Args)};
```