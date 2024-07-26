# Region

---

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
Region.Default.North_America; // => "na"
Region.Default.Latin_America; // => "latam"
Region.Default.Brazil; // => "br"
Region.Default.Public_Beta_Environment; // => "pbe"
Region.Default.Europe; // => "eu"
Region.Default.Korea; // => "kr"
Region.Default.Asia_Pacific; // => "ap"
```

_Example_

```typescript
new Client({
    region: Region.Default.Asia_Pacific
});
```
