# RiskReward TradingView v3.2

TradingView indicator written in **Pine Script v6** for visualizing LONG/SHORT trade plans imported from RiskReward mentor emails.

## Files

- `RiskReward_Trade_Viewer_v3.2.pine` — Pine Script source code.
- `RiskReward_Trade_Viewer_v3.2.txt` — identical source code in plain-text format, for devices/services that do not accept `.pine` downloads.

Both files contain **exactly the same code**. You only need one.

## Installation in TradingView

1. Open **TradingView**.
2. Go to **Supercharts**.
3. Click **Indicators**.
4. Select **My scripts**.
5. Click **Create new**.
6. Select **Indicator**.
7. Delete the default example code.
8. Open `RiskReward_Trade_Viewer_v3.2.pine` or `RiskReward_Trade_Viewer_v3.2.txt`.
9. Copy the entire code and paste it into the TradingView editor.
10. Click **Save** and name it `RiskReward Trade Viewer v3.2`.
11. Click **Add to chart**.

The indicator is now ready to use.

To import trades, open the indicator settings, paste the `TradingView Import` lines from a RiskReward mentor email into **Trades (paste TradingView Import)**, then select **Person (first trade #)** and **Trade within person #**.

**Import format** (one trade per line):

```text
TICKER,YYYY-MM-DD,L|S,ENTRY,STOP,TARGET,NAME,TRADER_ID
```

Example format (illustrative only):

```text
ORCL,2026-10-15,L,129.1,125,145,Trader Name,TR-00000001
```

## Notes

- The indicator groups trades by Trader ID and supports LONG and SHORT positions.
- The **Illustrative account value** and **Illustrative risk amount** inputs are for hypothetical position sizing; they are not the actual share count from the email.
- Pine Script drawings are not identical to TradingView's built-in draggable Long/Short Position tool.
- v3.2 has **not yet been confirmed as compiled and tested in TradingView**. Verify it in Pine Editor before relying on it.
- No example trades are preloaded.

## Publishing

Upload both source files and this README to a GitHub repository. The `.txt` version is intended for users who cannot download or handle `.pine` files. No license is granted by this README; add a LICENSE file separately if you want to specify reuse permissions.
