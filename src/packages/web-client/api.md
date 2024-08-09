# API

---

| Service                 | Function                  | Arguments                                     |
| ----------------------- | ------------------------- | --------------------------------------------- |
| **AccountXP**           | getPlayer                 | subject                                       |
| **Config**              | get                       |                                               |
| **Content**             | get                       |                                               |
| **ContractDefinitions** | getActiveStory            |                                               |
|                         | get                       |                                               |
|                         | getItemProgression        |                                               |
| **Contracts**           | get                       | subject                                       |
|                         | activate                  | subject, contractId                           |
|                         | unlockItemProgression     | subject, definitionId                         |
|                         | unlockContractProgression | subject, contractId                           |
|                         | unlockItemSidegrade       | subject, definitionId, sidegradeId, optionId  |
|                         | upgrade                   | subject, contractId                           |
| **CoreGame**            | fetchPlayer               | subject                                       |
|                         | fetchMatch                | matchId                                       |
|                         | fetchMatchLoadouts        | matchId                                       |
|                         | disassociatePlayer        | subject, matchId                              |
|                         | fetchAllChatMUCToken      | matchId                                       |
|                         | fetchTeamChatMUCToken     | matchId                                       |
|                         | fetchVoiceToken           | matchId                                       |
| **DailyTicket**         | get                       | subject                                       |
|                         | renew                     | subject                                       |
| **DisplayNameService**  | fetchPlayers              | subject                                       |
| **Favorites**           | get                       | subject                                       |
|                         | add                       | subject, itemId                               |
|                         | remove                    | subject, itemId                               |
| **Latency**             | fetchStats                |                                               |
|                         | fetchStat                 |                                               |
| **MassRewards**         | reconcilePlayer           | subject                                       |
| **Match**               | fetchMatchDetails         | matchId                                       |
|                         | fetchMatchHistory         | subject, queueId?, startIndex?, endIndex?     |
|                         | fetchQueueData            |                                               |
| **MMR**                 | getPlayer                 | subject                                       |
|                         | hideActRankBadge          | subject                                       |
|                         | getLeaderboard            | seasonId, startIndex?, size?, serachUsername? |
|                         | getCompetitiveUpdates     | subject, queueId?, startIndex?, endIndex?     |
| **Party**               | refreshCompetitiveTier    | subject, partyId                              |
|                         | refreshPlayerIdentity     | subject, partyId                              |
|                         | refreshPings              | subject, partyId                              |
|                         | get                       | partyId                                       |
|                         | getMUCToken               | partyId                                       |
|                         | getVoiceToken             | partyId                                       |
|                         | setAccessibility          | partyId, accessibility                        |
|                         | inviteByDisplayName       | partyId, gameName, tagLine                    |
|                         | declineJoinRequest        | partyId, requestId                            |
| **Party.MatchMaking**   | changeQueue               | partyId, queueId                              |
|                         | makeDefaultQueue          | partyId, queueId                              |
|                         | startSoloExperience       | subject                                       |
|                         | start                     | partyId                                       |
|                         | leave                     | partyId                                       |
| **Party.Player**        | get                       | subject                                       |
|                         | remove                    | subject                                       |
|                         | joinParty                 | subject, partyId                              |
|                         | leaveParty                | subject, partyId                              |
|                         | setReady                  | subject, partyId, isReady                     |
|                         | leaveFromParty            | subject, partyId                              |
|                         | transferOwner             | subject, partyId                              |
| **Party.CustomGame**    | makeInto                  | partyId                                       |
|                         | start                     | partyId                                       |
|                         | changeSettings            | partyId, settings                             |
|                         | changeTeam                | partyId, team, subject                        |
|                         | setBalance                | partyId                                       |
|                         | getConfig                 |                                               |
| **Party.PartyCode**     | create                    | partyId                                       |
|                         | delete                    | partyId                                       |
|                         | join                      | partyCode                                     |
| **Personalization**     | getPlayerLoadout          | subject                                       |
|                         | changePlayerLoadout       | subject, loadout                              |
| **PreGame**             | getPlayer                 | subject                                       |
|                         | getMatch                  | matchId                                       |
|                         | getMatchLoadouts          | matchId                                       |
|                         | selectCharacter           | matchId, agentId                              |
|                         | lockCharacter             | matchId, agentId                              |
|                         | fetchVoiceToken           | matchId                                       |
|                         | fetchChatToken            | matchId                                       |
|                         | quitMatch                 | matchId                                       |
| **Restrictions**        | fetchPlayerReportToken    | matchId, offenderSubject                      |
|                         | fetchPlayerRestrictions   |                                               |
| **Session**             | connect                   | subject                                       |
|                         | heartbeat                 | subject                                       |
|                         | disconnect                | subject                                       |
|                         | get                       | subject                                       |
|                         | reconnect                 | subject                                       |
| **Store**               | getWallet                 | subject                                       |
|                         | getOffers                 |                                               |
|                         | getEntitlements           | subject, itemTypeId                           |
| **Store.StoreFront**    | get                       | subject                                       |
|                         | revealNightMarketOffers   | subject                                       |
|                         | getAgent                  |                                               |

## Usage

```typescript
const data = await webClient.[Service].[Function]([Arguments]);
```
