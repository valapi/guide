# Client

---

```typescript
import { Auth } from "@valapi/auth";
```

## Config

```typescript
interface Config {
    /**
     * Authenticated User
     */
    user?: AuthUserInfo;

    /**
     * Riot Client SDK Version
     * 
     * ValorantApiCom.Internal.riotClientVersion() [riotGamesApiInfo.VS_FIXEDFILEINFO.FileVersion]
     */
    sdk?: 

    /**
     * Riot Client Build
     * 
     * ValorantApiCom.Version.get() [riotClientBuild]
     */
    build?: string;

    /**
     * Riot Client Version
     * 
     * ValorantApiCom.Version.get() [riotClientVersion]
     */
    version?: string;

    /**
     * Riot Client Platform
     * 
     * Where is Riot Client run on?
     */
    platform?: ClientPlatfrom;

    /**
     * Request Config
     */
    axiosConfig?: AxiosRequestConfig;

    /**
     * HTTPS Agent Config
     */
    agentConfig?: AgentOptions & CookieAgentOptions;
}
```

## Constructor

```typescript
const auth = new Auth( config? );
```

# Serialize

---

JSON

```typescript
const serializeJson = auth.toJSON();
```

Cookie

```typescript
const serializeCookie = auth.cookie.serializeSync();
```