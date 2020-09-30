# @capacitor/docgen

Docs Readme Markdown and JSON Generator for Capacitor Plugins.


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

-----------------

 ### notification

 ```typescript
 notification(options?: HapticsNotificationOptions | undefined) => Promise<string | number>
 ```

 Trigger a haptics "notification" feedback

 | Param       | Type                                                        |
 |-------------|-------------------------------------------------------------|
 | **options** | [`HapticsNotificationOptions`](#hapticsnotificationoptions) |

 **Returns:**  Promise<`string` \| `number`>


 ### vibrate

 ```typescript
 vibrate(options?: VibrateOptions | undefined) => Promise<number>
 ```

 Vibrate the device

 | Param       | Type                                |
 |-------------|-------------------------------------|
 | **options** | [`VibrateOptions`](#vibrateoptions) |

 **Returns:**  Promise<`number`>


 ### selectionStart

 ```typescript
 selectionStart(value: number | string) => Promise<void>
 ```

 Trigger a selection started haptic hint

 | Param     | Type                 |
 |-----------|----------------------|
 | **value** | `string` \| `number` |

 | Returns   |
 |-----------|
 | Promise<`void`> |

