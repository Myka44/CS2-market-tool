# CS2 Market Monitoring

A JavaFX desktop app for tracking CS2 item prices across CSFloat, DMarket and WhiteMarket. It stores price snapshots in SQLite so you can review price history and set alerts when prices reach a threshold.

## Run locally

Install JDK 21. From the repository root on Windows, run:

```powershell
.\gradlew.bat run
```

On Linux or macOS, run `./gradlew run`.

Use **Settings** to configure the marketplace integrations you want to use, then open **Price Monitor** or **Alerts**. The app stores its database locally at `.cs_auto_targets/data.db` in your home directory. Keep that database private because it also holds marketplace settings and credentials.

The **Targets** tab also supports automatic price adjustments. Enabling it for a target can create or update a live marketplace target.
