# Resources

-----------

```typescript
import {

    ItemTypeId,

    Locale,

    QueueId,

    Region,

}
from '@valapi/lib';
```

## Region

| Region | Full Name               |
| ------ | ----------------------- |
| na     | North_America           |
| latam  | Latin_America           |
| br     | Brazil                  |
| pbe    | Public_Beta_Environment |
| eu     | Europe                  |
| kr     | Korea                   |
| ap     | Asia_Pacific            |

# Usage

-----------

```typescript

[Resources].from. // string
[Resources].to. // readable

[Resources].toString('North_America'); // change readable to string
[Resources].fromString('na'); // change string to readable

```