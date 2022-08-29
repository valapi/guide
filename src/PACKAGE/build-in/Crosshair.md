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
interface LinesError {
    isEnable: boolean;
    Multiplier: number;
}
```

```typescript
interface Lines {
    isEnable: boolean,
    Opacity: number;
    Length: { // base on valorant settings
        Value: number;
        isChain: boolean;
        SecondValue: number;
    };
    Thickness: number;
    Offset: number;
    MovementError: Crosshair.LinesError;
    FiringError: Crosshair.LinesError;
}
```

```typescript
interface Crosshair {
    Primary: {
        Crosshair: {
            isHexCrosshairColor: boolean,
            CrosshairColor: string,
            OutLine: {
                isEnable: boolean,
                Opacity: number,
                Thickness: number,
            },
            CenterDot: {
                isEnable: boolean,
                Opacity: number,
                Thickness: number,
            },
            OverrideFiringErrorOffsetWithCrosshairOffset: boolean,
            OverrideAllPrimaryCrosshairWithMyPrimaryCrosshair: boolean,
        }
        InnerLines: Crosshair.Lines,
        OuterLines: Crosshair.Lines,
    };
    AimDownSights: {
        CopyPrimaryCrosshair: boolean,
        Crosshair: {
            isHexCrosshairColor: boolean,
            CrosshairColor: string,
            OutLine: {
                isEnable: boolean,
                Opacity: number,
                Thickness: number,
            },
            CenterDot: {
                isEnable: boolean,
                Opacity: number,
                Thickness: number,
            },
            OverrideFiringErrorOffsetWithCrosshairOffset: boolean,
        }
        InnerLines: Crosshair.Lines,
        OuterLines: Crosshair.Lines,
    };
    General: {
        Crosshair: {
            UseAdvancedOptions: boolean,
        },
        Other: {
            ShowSpectatedPlayerCrosshair: boolean,
            FadeCrosshairWithFiringError: boolean,
            DisableCrosshair?: boolean, // Not Usable
        },
    };
    SniperScope: {
        CenterDot: {
            isHexColor: boolean,
            Color: string,
            isEnable: boolean,
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