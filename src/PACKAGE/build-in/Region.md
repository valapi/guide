# Region

-----------

## Usage

```typescript
import { Region } from "valorant.ts";
```

```typescript
Region.North_America            // return "na"
Region.Latin_America            // return "latam"
Region.Brazil                   // return "br"
Region.Public_Beta_Environment  // return "pbe"
Region.Europe                   // return "eu"
Region.Korea                    // return "kr"
Region.Asia_Pacific             // return "ap"
```

*Example*

```typescript
new Client({

    region: Region.Asia_Pacific,

});
```