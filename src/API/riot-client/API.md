# API

-----------

| Service  | Function                                           | ...Args         |
| -------- | -------------------------------------------------- | --------------- |
| **Chat** | All_Chat_History                                   |                 |
|          | All_Chat_Info                                      |                 |
|          | All_Chat_Participants                              |                 |
|          | Game_Chat_Info                                     |                 |
|          | Party_Chat_Info                                    |                 |
|          | Pregame_Chat_Info                                  |                 |
|          | Specific_Chat_History                              | chatId          |
|          | TEXT_CHAT_RNet_FetchParticipants                   | chatId          |
|          | Send_Chat                                          | chatId, message |
|          | Send_Whisper                                       | chatId, message |
| **Main** | CHATFRIENDS_RNet_GET_ALL                           |                 |
|          | FRIENDS_RNet_FetchFriendRequests                   |                 |
|          | Local_Help                                         |                 |
|          | PRESENCE_RNet_GET_ALL                              |                 |
|          | PlayerAlias_RNet_GetActiveAlias                    |                 |
|          | RSO_Auth_User_Info                                 |                 |
|          | RSO_RNet_GetEntitlementsToken                      |                 |
|          | Riot_Client_Region                                 |                 |
|          | RiotClientSession_FetchSessions                    |                 |
|          | RiotKV_RNet_GetSettings                            |                 |
|          | RiotKV_RNet_GetSettingsTEXT_CHAT_RNet_FetchSession |                 |
| **More** | ANTI_ADDICTION_RNet_FetchShutdownPolicyState       |                 |
|          | ANTI_ADDICTION_RNet_FetchWarningMessagePolicyState |                 |
|          | CLIENTCONFIG_RNET_GET_ValorantClientConfig         |                 |
|          | LEGAL_INFO_RNet_EULA                               |                 |
|          | LEGAL_INFO_RNet_Privacy                            |                 |
|          | LOCALE_RNet_FetchAvailableLocales                  |                 |
|          | LOCALE_RNet_FetchLocale                            |                 |
|          | Local_Swagger_Docs                                 |                 |
|          | REPORTER_FEEDBACK_RNet_GetReporterFeedback         |                 |
|          | RIOT_WARNING_RNet_GetRiotWarning                   |                 |
|          | RSO_RNet_FetchClientAuthorizations                 |                 |
|          | RSO_RNet_GetAccessToken                            |                 |
|          | RSO_RNet_GetUserInfoToken                          |                 |
|          | Riot_Client_Command_Line_Args                      |                 |
|          | RiotStatus_RNet_FetchStatus                        | region          |
|          | TEXT_CHAT_RNet_FetchSettings                       |                 |
|          | TEXT_CHAT_RNet_GetMUCInfos_coregame                |                 |
|          | TEXT_CHAT_RNet_GetMUCInfos_parties                 |                 |
|          | TEXT_CHAT_RNet_GetMUCInfos_pregame                 |                 |
|          | TEXT_CHAT_RNet_GetMUCInfos_tournaments             |                 |
|          | URNetClient_CheckPluginStatus                      |                 |
|          | URNetClient_CheckRMSSession                        |                 |
|          | URNetClient_GetProcessInfo                         |                 |
|          | VOICE_CHAT_RNet_FetchAudioProperties               |                 |
|          | VOICE_CHAT_RNet_FetchCaptureDevices                |                 |
|          | VOICE_CHAT_RNet_FetchPTTSettings                   |                 |
|          | VOICE_CHAT_RNet_FetchRenderDevices                 |                 |
|          | VOICE_CHAT_RNet_FetchSessions                      |                 |
|          | VOICE_CHAT_RNet_FetchSettings                      |                 |
|          | Valorant_Log_Path                                  |                 |
  
## Usage

```typescript
    const _data = await ApiClient.{Service}.{Function(...Args)};
```