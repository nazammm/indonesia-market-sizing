# Data

Both files are compilations of public BPS (Statistics Indonesia) tables at regency and city level. Neither is a raw BPS download: BPS publishes these as separate dynamic tables, and the two repositories below joined them into one row per region.

| File | Contents | Compiled by |
|---|---|---|
| `raw/bps_kabkota_2025.csv` | Population, adjusted per-capita expenditure, HDI, poverty rate, unemployment and construction cost index (IKK) for 514 regions, 2025 | [bilbobib/IPM-Viz](https://github.com/bilbobib/IPM-Viz) |
| `raw/bps_kabkota_2024_location_growth.csv` | Real GRDP growth 2024 and region centroid coordinates | [ariantobarus123/uas-visdat-stis-2026](https://github.com/ariantobarus123/uas-visdat-stis-2026) (`data/master_data_2024.csv`, columns cut to the ones used here) |
| `raw/bps_kabkota_2025_sources.csv` | The BPS table behind each column | |

Notes:

- Seven region names are spelled differently between the two files (for example `Kota Makasar` / `Kota Makassar`, `Toba Samosir / Toba` / `Toba Samosir`). The notebook maps them explicitly and checks that every region matches.
- Three regions have no coordinates and are left off the maps. They are still scored.
- The 2024 file also has GRDP levels, but its compiler notes that their units were not verified, so they are not used.
