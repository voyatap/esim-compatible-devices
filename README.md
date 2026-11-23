# eSIM Compatible Devices Dataset (VoyaTap)

An open, manufacturer-verified dataset of **265 phones, tablets, and smartwatches across 15 brands**, maintained by [VoyaTap](https://voyatap.com/en) and published under **CC BY 4.0**.

- **Interactive web directory**: [https://voyatap.com/en/devices](https://voyatap.com/en/devices)
- **Interactive eSIM compatibility checker**: [https://voyatap.com/en/tools/esim-checker](https://voyatap.com/en/tools/esim-checker)
- **Machine-readable files**: [`data/devices.json`](./data/devices.json) · [`data/devices.csv`](./data/devices.csv) · [`data/schema.json`](./data/schema.json)
- **First published**: 2026-04-12 · **Last verified**: 2026-09-14

## Why this dataset exists

Many third-party compatibility tables silently copy outdated lists and mislabel incompatible phones or regional hardware variants. This dataset includes:

1. **Honest negative entries (30 models with `esim_supported: false`)** — devices frequently misreported elsewhere as eSIM-compatible (such as Huawei Mate 60 Pro, Xiaomi 14 Ultra, ASUS ROG Phone 8, Nothing Phone (2), Galaxy Tab S8, and Garmin watches).
2. **Travel eSIM usability (`travel_esim_usable`)** — explicitly distinguishes cellular smartwatches (which carry carrier-locked eSIMs and cannot install third-party travel data profiles) from phones and cellular tablets (**219** travel-eSIM-usable models out of **235** hardware-eSIM models).
3. **Regional hardware caveats (English + Simplified Chinese)** — documents mainland-China dual-physical-SIM variants, US and 12-region eSIM-only iPhones, and cellular-only tablets.

## Brand summary

| Brand | Total models | eSIM hardware | Honest `no eSIM` |
| --- | ---: | ---: | ---: |
| [Apple](https://voyatap.com/en/devices#apple) | 69 | 69 | 0 |
| [Samsung](https://voyatap.com/en/devices#samsung) | 67 | 64 | 3 |
| [Google](https://voyatap.com/en/devices#google) | 33 | 33 | 0 |
| [OnePlus](https://voyatap.com/en/devices#oneplus) | 8 | 7 | 1 |
| [Xiaomi](https://voyatap.com/en/devices#xiaomi) | 15 | 10 | 5 |
| [OPPO](https://voyatap.com/en/devices#oppo) | 13 | 10 | 3 |
| [Motorola](https://voyatap.com/en/devices#motorola) | 13 | 13 | 0 |
| [Sony](https://voyatap.com/en/devices#sony) | 6 | 6 | 0 |
| [Nothing](https://voyatap.com/en/devices#nothing) | 7 | 3 | 4 |
| [Honor](https://voyatap.com/en/devices#honor) | 7 | 7 | 0 |
| [Huawei](https://voyatap.com/en/devices#huawei) | 5 | 1 | 4 |
| [ASUS](https://voyatap.com/en/devices#asus) | 7 | 3 | 4 |
| [vivo](https://voyatap.com/en/devices#vivo) | 7 | 6 | 1 |
| [Microsoft](https://voyatap.com/en/devices#microsoft) | 3 | 3 | 0 |
| [Garmin](https://voyatap.com/en/devices#garmin) | 5 | 0 | 5 |

## Models verified as NOT supporting eSIM (30)

| Brand | Model | Year | Category | Verification note |
| --- | --- | ---: | --- | --- |
| Samsung | [Galaxy Tab S8 Ultra](https://voyatap.com/en/devices/samsung-galaxy-tab-s8-ultra) | 2022 | tablet | Samsung's eSIM device list begins at the Tab S9 — the Tab S8 5G takes a physical nano-SIM only, in every region. Third-party lists marking this model eSIM-capable are wrong. |
| Samsung | [Galaxy Tab S8+](https://voyatap.com/en/devices/samsung-galaxy-tab-s8-plus) | 2022 | tablet | Samsung's eSIM device list begins at the Tab S9 — the Tab S8 5G takes a physical nano-SIM only, in every region. Third-party lists marking this model eSIM-capable are wrong. |
| Samsung | [Galaxy Tab S8](https://voyatap.com/en/devices/samsung-galaxy-tab-s8) | 2022 | tablet | Samsung's eSIM device list begins at the Tab S9 — the Tab S8 5G takes a physical nano-SIM only, in every region. Third-party lists marking this model eSIM-capable are wrong. |
| OnePlus | [12R](https://voyatap.com/en/devices/oneplus-12r) | 2024 | phone | Global/EU/India models are dual physical SIM with no eSIM; only the North America model (CPH2611) is reported to support eSIM. |
| Xiaomi | [15 Pro](https://voyatap.com/en/devices/xiaomi-15-pro) | 2025 | phone | China-only model — never sold globally; dual physical nano-SIM, no eSIM. |
| Xiaomi | [14 Ultra](https://voyatap.com/en/devices/xiaomi-14-ultra) | 2024 | phone | No eSIM on any variant, including the global version — unlike the global Xiaomi 14. Dual physical nano-SIM only. |
| Xiaomi | [14 Pro](https://voyatap.com/en/devices/xiaomi-14-pro) | 2023 | phone | China-only model — never sold globally; dual physical nano-SIM, no eSIM. |
| Xiaomi | [13 Ultra](https://voyatap.com/en/devices/xiaomi-13-ultra) | 2023 | phone | The global 13 Ultra has no eSIM — unlike the global Xiaomi 13 / 13 Pro. Dual physical nano-SIM only. |
| Xiaomi | [Mix Fold 4](https://voyatap.com/en/devices/xiaomi-mix-fold-4) | 2024 | phone | China-only; dual physical nano-SIM. No global variant was ever released. |
| OPPO | [Find X8 Ultra](https://voyatap.com/en/devices/oppo-find-x8-ultra) | 2025 | phone | China-only model; no standard eSIM (OPPO's ORoaming app cannot install third-party travel eSIM profiles). |
| OPPO | [Reno 12 Pro 5G](https://voyatap.com/en/devices/oppo-reno-12-pro-5g) | 2024 | phone | Dual physical nano-SIM only — the Reno 12 generation skipped eSIM (it returned on Reno 13/14). |
| OPPO | [Reno 12 5G](https://voyatap.com/en/devices/oppo-reno-12-5g) | 2024 | phone | Dual physical nano-SIM only — the Reno 12 generation skipped eSIM (it returned on Reno 13/14). |
| Nothing | [Phone (2a) Plus](https://voyatap.com/en/devices/nothing-phone-2a-plus) | 2024 | phone | Dual physical nano-SIM only — no eSIM in any region. |
| Nothing | [Phone (2a)](https://voyatap.com/en/devices/nothing-phone-2a) | 2024 | phone | Dual physical nano-SIM only — no eSIM in any region. |
| Nothing | [Phone (2)](https://voyatap.com/en/devices/nothing-phone-2) | 2023 | phone | Dual physical nano-SIM only — no eSIM in any region (confirmed by Nothing's official support pages). |
| Nothing | [Phone (1)](https://voyatap.com/en/devices/nothing-phone-1) | 2022 | phone | Dual physical nano-SIM only — no eSIM in any region (confirmed by Nothing's official support pages). |
| Huawei | [Pura 70 Ultra](https://voyatap.com/en/devices/huawei-pura-70-ultra) | 2024 | phone | Dual physical nano-SIM only — no eSIM on any variant. |
| Huawei | [Pura 70 Pro](https://voyatap.com/en/devices/huawei-pura-70-pro) | 2024 | phone | Dual physical nano-SIM only — no eSIM on any variant. |
| Huawei | [Mate 60 Pro](https://voyatap.com/en/devices/huawei-mate-60-pro) | 2023 | phone | Dual physical nano-SIM only — no eSIM on any variant. (Compatibility lists claiming eSIM support for this model are wrong.) |
| Huawei | [P50 Pro](https://voyatap.com/en/devices/huawei-p50-pro) | 2021 | phone | eSIM was only available via an optional snap-on 5G case accessory — the phone itself has no built-in eSIM. No Google services. |
| ASUS | [ROG Phone 8 Pro](https://voyatap.com/en/devices/asus-rog-phone-8-pro) | 2024 | phone | Dual physical nano-SIM only — no eSIM. ASUS's first eSIM phones are the ROG Phone 9 series and Zenfone 12 Ultra. |
| ASUS | [ROG Phone 8](https://voyatap.com/en/devices/asus-rog-phone-8) | 2024 | phone | Dual physical nano-SIM only — no eSIM. ASUS's first eSIM phones are the ROG Phone 9 series and Zenfone 12 Ultra. |
| ASUS | [Zenfone 11 Ultra](https://voyatap.com/en/devices/asus-zenfone-11-ultra) | 2024 | phone | Dual physical nano-SIM only — no eSIM. ASUS's first eSIM phones are the ROG Phone 9 series and Zenfone 12 Ultra. |
| ASUS | [Zenfone 10](https://voyatap.com/en/devices/asus-zenfone-10) | 2023 | phone | Dual physical nano-SIM only — no eSIM. ASUS's first eSIM phones are the ROG Phone 9 series and Zenfone 12 Ultra. |
| vivo | [X Fold 3 Pro](https://voyatap.com/en/devices/vivo-x-fold-3-pro) | 2024 | phone | No eSIM on any variant (dual physical nano-SIM), including the global/India version. |
| Garmin | [Fenix 8 Pro](https://voyatap.com/en/devices/garmin-fenix-8-pro) | 2025 | wearable | Garmin's first watch with cellular (LTE) alongside inReach satellite messaging — but the embedded SIM is tied to Garmin's own subscription, activated in Garmin Connect. No carrier or travel eSIM profile can be installed, and Garmin sells the service in a limited list of countries. |
| Garmin | [Forerunner 945 LTE](https://voyatap.com/en/devices/garmin-forerunner-945-lte) | 2021 | wearable | The LTE here is Garmin's own subscription service activated through Garmin Connect, not a carrier eSIM — travel eSIMs cannot be installed. Availability is limited to the countries Garmin lists for the service. |
| Garmin | [Fenix 8](https://voyatap.com/en/devices/garmin-fenix-8) | 2024 | wearable | No cellular radio at all — Garmin's first watches with cellular are the fēnix 8 Pro series (2025). Connectivity comes from a paired phone. |
| Garmin | [Forerunner 965](https://voyatap.com/en/devices/garmin-forerunner-965) | 2023 | wearable | No cellular radio and no eSIM — Garmin never shipped an LTE version of the 965. It connects through a paired phone. |
| Garmin | [Forerunner 955](https://voyatap.com/en/devices/garmin-forerunner-955) | 2022 | wearable | No cellular radio and no eSIM — Garmin never shipped an LTE version of the 955. It connects through a paired phone. |

## Files & schema

- `data/devices.json` — structured JSON object with dataset metadata and all 265 entries.
- `data/devices.csv` — flat RFC 4180 CSV table for spreadsheets, pandas, DuckDB, or SQL imports.
- `data/schema.json` — JSON Schema (Draft 2020-12) validating `data/devices.json`.

Every record includes a canonical `voyatap_url` linking directly to that model's full bilingual/trilingual specification and setup guide on `voyatap.com`.

## Primary manufacturer sources

- **Apple**: [Apple Support — SIM types on iPhone and iPad](https://support.apple.com/en-us/118569)
- **Samsung**: [Samsung Support — Galaxy eSIM compatibility](https://www.samsung.com/au/support/mobile-devices/esim-compatibility/)
- **Google**: [Google Support — eSIMs on Pixel phones](https://support.google.com/pixelphone/answer/16115741)
- **Garmin**: [Garmin — LTE and satellite connectivity](https://www.garmin.com/en-US/connectivity/)
- **Other brands**: Official manufacturer specification pages and regional support documentation.

## Changelog

- **2026-09-14**: Apple's September 2026 lineup added from Apple's own spec pages: iPhone 18 Pro and 18 Pro Max (eSIM-only in the same 12 countries/regions as the 17 Pro; the mainland-China models A3715/A3718 are the first Pro iPhones with eSIM in China), iPhone Duo (Apple's first foldable, eSIM-only in every market with no SIM tray at all, on sale 23 Oct), Apple Watch Series 12 and Ultra 4. The iPhone Air and 17e entries no longer call themselves the "only two" iPhones with eSIM in China — that stopped being true this month. The non-Pro iPhone 18, 18e and Air 2 are not listed: Apple has them slated for spring 2027 and has published no specs.
- **2026-08-20**: Tablet and wearable coverage extended, both directions. Added the 11 Galaxy tablets Samsung's own eSIM list names (Tab S11, S10+/S10 Ultra, S10 FE/FE+, S9/S9+/S9 Ultra, S9 FE/FE+, Tab Active5/Active5 Pro) — and, because that list starts at the Tab S9, added Galaxy Tab S8/S8+/S8 Ultra as honest "no eSIM" entries, correcting a claim several third-party lists get wrong. Added 5 Garmin watches, all honest "no": the fēnix 8 Pro and Forerunner 945 LTE do carry an embedded SIM, but it is locked to Garmin's own subscription and no travel eSIM can be written to it; the fēnix 8, Forerunner 965 and 955 have no cellular radio at all. realme and ZTE were researched and deliberately left out — neither publishes an official eSIM device list, and the third-party sources contradict each other.
- **2026-08-10**: Full re-verification of every entry against manufacturer sources. Added 71 devices released through Aug 2026 (iPhone Air/16e/17e, Pixel 10 series, Galaxy S26 & Z Fold 8 series, Xiaomi 17 series and more). Corrected eSIM-only labeling to be region-accurate (US-only for iPhone 14–16; 12 regions for iPhone 17), dual-eSIM counts (Galaxy S24+, Pixel 7+), and — importantly — 22 entries that do NOT support eSIM (all previous ASUS/Huawei/Nothing listings, several Xiaomi/OPPO models) now say so honestly. Reference-page upgrades (anchors, source links, citation guidance) shipped the same day.
- **2026-04-12**: Initial dataset published; every entry checked against manufacturer spec pages.

## License & citation

This dataset is licensed under **Creative Commons Attribution 4.0 International (CC BY 4.0)** — see [`LICENSE`](./LICENSE).

You are free to share, copy, and adapt this dataset for any purpose (including commercial tools, articles, and AI applications) provided you give appropriate attribution:

> Data source: VoyaTap eSIM Device Compatibility Database (last verified 2026-09-14), https://voyatap.com/en/devices, licensed under CC BY 4.0.
