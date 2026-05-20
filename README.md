# Forza Horizon 6 — SimHub Resources

Community resources for Forza Horizon 6, focused on SimHub integration and modding tools.

## Car ID Mapping — `carNames.json`

Maps internal car IDs (e.g. `Car_1006`) to human-readable names and media asset names for all cars in the game.

**638 cars** currently mapped.

### Format

```json
{
  "Car_1006": {
    "mediaName": "FER_FXX_05",
    "name": "2005 Ferrari FXX"
    "shortName": "2005 Ferrari FXX"
    "make": "Ferrari"
  }
}
```

| Field | Description |
|-------|-------------|
| Key (`Car_XXXX`) | Internal game car ID as reported by SimHub telemetry |
| `name` | Full display name of the car |
| `make` | Make of the car |
| `shortName` | Short display name of the car |
| `mediaName` | Internal asset/media identifier used by the game |

### Usage

Use `carNames.json` in SimHub dashboards or overlays to resolve the car ID from telemetry into a readable car name. The `mediaName` field can be used to load car livery images or other media assets where available.

## Contributing

If you find a missing or incorrectly named car, pull requests are welcome. Add the entry to `carNames.json` in alphabetical key order (`Car_XXXX`).
