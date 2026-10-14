## 2022-08-25

For Baidu and Huawei APP Market audit `onCordovaReady`, don't get uuid automatically, provide another method `getUuid` to get it.

## 2026-10-14

1. Remove `getUuid`.
2. Add `DeviceAutoGetInfo` to control whether `getInfo` runs on `onCordovaReady`, preventing sensitive information collection before user consent.

Configure `DeviceAutoGetInfo` in `capacitor.config.json`:

```json
{
  "cordova": {
    "preferences": {
      "DeviceAutoGetInfo": false
    }
  }
}
```
