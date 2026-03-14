# MCSR Ranked ELO Overlay

<p align="center">
  <img width="174" height="240" alt="MCSR_Overlay_Icon" src="https://github.com/user-attachments/assets/1dc8ca19-46fd-48f3-bfdc-31486bcfe130" />
</p>

A live ELO tracker overlay for [MCSR Ranked](https://mcsrranked.com) — designed for use in OBS as a browser source.

---

## Features

- **Live ELO display** with animated slot-machine digit rolling
- **Rank icon & name** with animated shard/shatter effect on rank-up
- **Season stats** — wins, losses, win rate with progress bar, and best time
- **Rank tiers** — Coal, Iron, Gold, Emerald, Diamond, Netherite
- **Settings panel** — enter and save your username directly in the overlay, no file editing needed
- **Persistent username** — saved via `localStorage`, survives OBS restarts

---

## Setup

### OBS Browser Source

1. In OBS, click **+** under Sources and select **Browser**
2. Check **Local file** and browse to `MCSR_overlay.html`
3. Set **Width** to `420` and **Height** to `450` (The window may need cropping to get rid of black boxes. The height must be this high to use the full dropdowns)
4. Click **OK**


### First-time Username Setup

When you load the overlay for the first time, a settings panel will open automatically. Enter your MCSR Ranked username and click **SAVE**. Your username is stored in `localStorage` and will be remembered across sessions.

---

## Changing Your Username

There are three ways to open the settings panel at any time:

- Click the **⚙** gear icon in the top-right corner of the overlay
- Click on your **username** in the overlay header
- The settings panel opens automatically if no username is set

Press **Enter** to save, **Escape** or click outside the modal to cancel.

---



## Data Source

Stats are fetched from the [MCSR Ranked public API](https://mcsrranked.com) and refreshed every second. No API key is required.

---
> **Disclaimer:** This project is an independent, community-made tool and is not affiliated with, endorsed by, or associated with the official MCSR Ranked team in any way.

