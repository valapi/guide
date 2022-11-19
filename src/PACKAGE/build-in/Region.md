# Region

-----------

## Usage

```typescript
import { Region } from "@valapi/lib";
```

## Usage

| Region | Full Name               |
| ------ | ----------------------- |
| na     | North_America           |
| latam  | Latin_America           |
| br     | Brazil                  |
| pbe    | Public_Beta_Environment |
| eu     | Europe                  |
| kr     | Korea                   |
| ap     | Asia_Pacific            |

```typescript
Region.Default.North_America            // return "na"
Region.Default.Latin_America            // return "latam"
Region.Default.Brazil                   // return "br"
Region.Default.Public_Beta_Environment  // return "pbe"
Region.Default.Europe                   // return "eu"
Region.Default.Korea                    // return "kr"
Region.Default.Asia_Pacific             // return "ap"
```

*Example*

```typescript
new Client({

    region: Region.Default.Asia_Pacific,

});
```