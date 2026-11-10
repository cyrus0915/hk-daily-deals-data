# Hong Kong Daily Deals — Public Read-Only Data

This repository holds public read-only data synced from the private Hong Kong daily deals board （香港日常優惠）.

- `deals.json` contains the current live deals: store, item, price, category, details, source, original post text, and expiry where available, plus headline stats (`totalLive`, `categoryCounts`, `bestDiscountPct`, `todayNew`, `sourceTotal`, `lastUpdatedAt`, `syncedAt`).
- The public deals page reads `deals.json` from this repository at load time, so visitors always see the latest synced data without the page itself needing to be rebuilt or re-published.
- Visitors can read this data but not edit it. Only the board owner can update this repository; there is no public editing, submission, or write access.
- Updated about every 2 hours, following the private board's refresh cycle.
