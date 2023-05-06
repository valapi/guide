# API

---

| Service                 | Function                   | Arguments                                     |
| ----------------------- | -------------------------- | --------------------------------------------- |
| **AccountXP**           | getPlayer                  | subject                                       |
| **Config**              | fetchConfig                |                                               |
| **Content**             | fetchContent               |                                               |
| **ContractDefinitions** | fetchActiveStory           |                                               |
|                         | fetch                      |                                               |
|                         | fetchItemProgression       |                                               |
| **Contracts**           | fetch                      | subject                                       |
|                         | activate                   | subject, contractId                           |
|                         | unlockItemProgress         | subject, definitionId                         |
|                         | unlockContractProgression  | subject, contractId                           |
|                         | unlockItemSidegrade        | subject, definitionId, sidegradeId, optionId  |
|                         | upgrade                    | subject, contractId                           |
| **CoreGame**            | fetchPlayer                | subject                                       |
|                         | fetchMatch                 | matchId                                       |
|                         | fetchMatchLoadouts         | matchId                                       |
|                         | disassociatePlayer         | subject, matchId                              |
|                         | fetchAllChatMUCToken       | matchId                                       |
|                         | fetchTeamChatMUCToken      | matchId                                       |
|                         | fetchVoiceToken            | matchId                                       |
| **DisplayNameService**  | fetchPlayers               | subject                                       |
| **Favorites**           | get                        | subject                                       |
|                         | add                        | subject, itemId                               |
|                         | remove                     | subject, itemId                               |
| **Latency**             | fetchStats                 |                                               |
|                         | fetchStat                  |                                               |
| **MassRewards**         | reconcilePlayer            | subject                                       |
| **Match**               | fetchMatchDetails          | matchId                                       |
|                         | fetchMatchHistory          | subject, queueId?, startIndex?, endIndex?     |
|                         | fetchQueueData             |                                               |
| **MMR**                 | fetchPlayer                | subject                                       |
|                         | hideActRankBadge           | subject                                       |
|                         | fetchLeaderboard           | seasonId, startIndex?, size?, serachUsername? |
|                         | fetchCompetitiveUpdates    | subject, queueId?, startIndex?, endIndex?     |
| **Party**               | fetchPlayer                | subject                                       |
|                         | removePlayer               | subject                                       |
|                         | joinParty                  | subject, partyId                              |
|                         | leaveParty                 | subject, partyId                              |
|                         | setMemberReady             | subject, partyId, isReady                     |
|                         | refreshCompetitiveTier     | subject, partyId                              |
|                         | refreshPlayerIdentity      | subject, partyId                              |
|                         | refreshPings               | subject, partyId                              |
|                         | fetchParty                 | partyId                                       |
|                         | leaveFromParty             | subject, partyId                              |
|                         | fetchMUCToken              | partyId                                       |
|                         | fetchVoiceToken            | partyId                                       |
|                         | makeIntoCustomGame         | partyId                                       |
|                         | changeQueue                | partyId, queueId                              |
|                         | makeDefault                | partyId, queueId                              |
|                         | startCustomGame            | partyId                                       |
|                         | startSoloExperience        | subject                                       |
|                         | setCustomGameSettings      | partyId, settings                             |
|                         | changeTeamInCustomGame     | partyId, team, subject                        |
|                         | enterMatchmakingQueue      | partyId                                       |
|                         | leaveMatchmakingQueue      | partyId                                       |
|                         | setAccessibility           | partyId, accessibility                        |
|                         | inviteToPartyByDisplayName | partyId, gameName, tagLine                    |
|                         | declineRequest             | partyId, requestId                            |
|                         | setBalance                 | partyId                                       |
|                         | fetchCustomGameConfigs     |                                               |
|                         | transferOwner              | subject, partyId                              |
| **Personalization**     | getPlayerLoadout           | subject                                       |
|                         | playerLoadoutUpdate        | subject, loadout                              |
| **PreGame**             | getPlayer                  | subject                                       |
|                         | getMatch                   | matchId                                       |
|                         | getMatchLoadouts           | matchId                                       |
|                         | selectCharacter            | matchId, agentId                              |
|                         | lockCharacter              | matchId, agentId                              |
|                         | fetchVoiceToken            | matchId                                       |
|                         | fetchChatToken             | matchId                                       |
|                         | quitMatch                  | matchId                                       |
| **Restrictions**        | fetchPlayerReportToken     | matchId, offenderSubject                      |
|                         | fetchPlayerRestrictions    |                                               |
| **Session**             | connect                    | subject                                       |
|                         | heartbeat                  | subject                                       |
|                         | disconnect                 | subject                                       |
|                         | get                        | subject                                       |
|                         | reconnect                  | subject                                       |
| **Store**               | getWallet                  | subject                                       |
|                         | getStorefront              | subject                                       |
|                         | getOffers                  |                                               |
|                         | getEntitlements            | subject, itemTypeId                           |
|                         | revealNightMarketOffers    | subject                                       |

## Usage

```typescript
const data = await webClient.Service.Function(...Arguments);
```
