
# Haptics

The Haptics API provides physical feedback to the user through touch or vibration.

<!--DOCGEN_INDEX_START-->
* [impact()](#impact)
* [notification()](#notification)
* [vibrate()](#vibrate)
* [selectionStart()](#selectionstart)
<!--DOCGEN_INDEX_END-->

## Android Notes

To use vibration, you must add this permission to your `AndroidManifest.xml` file:

```xml
<uses-permission android:name="android.permission.VIBRATE" />
```

## Example

```typescript
import {
  Plugins,
  HapticsImpactStyle
} from '@capacitor/core';

const { Haptics } = Plugins;

export class HapticsExample {
  hapticsImpact(style = HapticsImpactStyle.Heavy) {
    Haptics.impact({
      style: style
    });
  }

  hapticsImpactMedium(style) {
    this.hapticsImpact(HapticsImpactStyle.Medium);
  }

  hapticsImpactLight(style) {
    this.hapticsImpact(HapticsImpactStyle.Light);
  }

  hapticsVibrate() {
    Haptics.vibrate();
  }

  hapticsSelectionStart() {
    Haptics.selectionStart();
  }

  hapticsSelectionChanged() {
    Haptics.selectionChanged();
  }

  hapticsSelectionEnd() {
    Haptics.selectionEnd();
  }
}
```

<!--DOCGEN_API_START-->
## API

### impact

```typescript
impact(options: HapticsImpactOptions, x?: number | undefined) => Promise<HapticsImpact>
```

Trigger a haptics "impact" feedback

| Param       | Type                                            | Description        |
|-------------|-------------------------------------------------|--------------------|
| **options** | [`HapticsImpactOptions`](#hapticsimpactoptions) | The impact options |
| **x**       | `number`                                        |                    |

**Returns:**  Promise<[`HapticsImpact`](#hapticsimpact)>

--------------------


### notification

```typescript
notification(options?: HapticsNotificationOptions | undefined) => Promise<string | number>
```

Trigger a haptics "notification" feedback

| Param       | Type                                                        |
|-------------|-------------------------------------------------------------|
| **options** | [`HapticsNotificationOptions`](#hapticsnotificationoptions) |

**Returns:**  Promise<`string` \| `number`>

--------------------


### vibrate

```typescript
vibrate(options?: VibrateOptions | undefined) => Promise<number>
```

Vibrate the device

| Param       | Type                                |
|-------------|-------------------------------------|
| **options** | [`VibrateOptions`](#vibrateoptions) |

**Returns:**  Promise<`number`>

--------------------


### selectionStart

```typescript
selectionStart(value: number | string) => Promise<void>
```

Trigger a selection started haptic hint

| Param     | Type                 |
|-----------|----------------------|
| **value** | `string` \| `number` |

**Returns:**  Promise<`void`>

--------------------


### Interfaces


#### HapticsImpact


--------------------


#### HapticsImpactOptions


--------------------


#### HapticsNotificationOptions


--------------------


#### VibrateOptions


--------------------


### Enums


<!--DOCGEN_API_END-->
