# Crosshair Compiler

*beta*

-----------

## Client

```typescript
import { Crosshair } from "valorant.ts";
```

```typescript
const MyCrosshair = new Crosshair( CrosshairCode? );
```

## Usage

Get new crosshair code

```typescript
MyCrosshair.toJson(); // json format
```

```typescript
MyCrosshair.toString(); // crosshair code
```

## Settings

All settings are based on in-game

```typescript
interface CrosshairLinesError {
    isEnable: Boolean; // Not in Valorant settings
    Multiplier: number;
}
```

```typescript
interface CrosshairLines {
    isEnable: Boolean, // Not in Valorant settings
    Opacity: number;
    Length: number;
    Thickness: number;
    Offset: number;
    MovementError: CrosshairLinesError;
    FiringError: CrosshairLinesError;
}
```

```typescript
interface Crosshair {
    Primary: {
        Crosshair: {
            CrosshairColor: number,
            OutLine: {
                isEnable: Boolean, // Not in Valorant settings
                Opacity: number,
                Thickness: number,
            },
            CenterDot: {
                isEnable: Boolean, // Not in Valorant settings
                Opacity: number,
                Thickness: number,
            },
            OverrideFiringErrorOffsetWithCrosshairOffset: Boolean,
            OverrideAllPrimaryCrosshairWithMyPrimaryCrosshair: Boolean,
        }
        InnerLines: CrosshairLines,
        OuterLines: CrosshairLines,
    };
    AimDownSights: {
        CopyPrimaryCrosshair: Boolean,
        Crosshair: {
            CrosshairColor: number,
            OutLine: {
                isEnable: Boolean, // Not in Valorant settings
                Opacity: number,
                Thickness: number,
            },
            CenterDot: {
                isEnable: Boolean, // Not in Valorant settings
                Opacity: number,
                Thickness: number,
            },
            OverrideFiringErrorOffsetWithCrosshairOffset: Boolean,
        }
        InnerLines: CrosshairLines,
        OuterLines: CrosshairLines,
    };
    General: {
        Crosshair: {
            UseAdvancedOptions: Boolean,
        },
        Other: {
            ShowSpectatedPlayerCrosshair: Boolean,
            FadeCrosshairWithFiringError: Boolean,
            DisableCrosshair?: Boolean, // Not Usable
        },
    };
    SniperScope: {
        CenterDot: {
            Color: number,
            isEnable: Boolean, // Not in Valorant settings
            Opacity: number,
            Thickness: number,
        },
    };
}
```

*Example*

```typescript
MyCrosshair.Primary.InnerLines.Thickness = 2;
```