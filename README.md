# tb_tow_sale_point

A QBCore script for FiveM that allows players with specific jobs to tow vehicles to designated locations and sell them for a random cash or bank payout.

## Features
- Multiple sale locations with blips and markers
- Configurable allowed jobs and vehicles
- Random payout within a configurable range
- Only allowed jobs can sell towed vehicles

## Installation
1. Place the `tb_tow_sale_point` folder in your server's `resources` directory.
2. Add `ensure tb_tow_sale_point` to your `server.cfg`.
3. Make sure you are using QBCore.

## Configuration
Edit `config.lua` to customize:
- **AllowedJobs**: List of jobs that can sell vehicles
- **SaleLocations**: Add or remove sale points (vector3)
- **AllowedVehicles**: List of tow vehicle models
- **PayoutType**: "cash" or "bank"
- **MinPrice/MaxPrice**: Sale price range
- **Blip/Marker**: Visual settings

Example for multiple jobs and locations:
```lua
Config.AllowedJobs = {
    "tow",
    "mechanic",
}
Config.SaleLocations = {
    vector3(235.0, -800.0, 30.0),
    vector3(-428.0, -1728.0, 19.0),
    vector3(1208.0, -3115.0, 5.5),
}
```

## Usage
1. Get in an allowed tow vehicle with a towed car attached.
2. Drive to a sale location (marked on the map).
3. Press `E` at the marker to sell the towed vehicle and receive a payout.

## Support
If you have issues or want more features, open an issue or contact the script author.
