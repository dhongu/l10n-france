# l10n-france

Localizare Odoo pentru Franța (Terrabit).

## Module

- `l10n_fr_zip` — localitățile (French) cu codul poștal, legate de regiunile țării; completează localitatea
  și regiunea din codul poștal și leagă contactele existente de localitatea codului lor poștal: la
  instalare, direct pe o bază mică sau printr-o acțiune programată, pe loturi, pe una mare.

## Date

Lista de localități vine din [GeoNames](https://www.geonames.org) (licență Creative Commons
Attribution 4.0). Pentru reîmprospătare:

```bash
curl -sSfLO https://download.geonames.org/export/zip/FR.zip && unzip FR.zip FR.txt
python3 scripts/generate_city_data.py FR.txt
```
