# SPPG Distribution Maps

[map_highlight](docs/map_highlight.png)

Dikarenakan rasa penasaran + gabut saya serta tidak adanya kepastian mengenai peta sebaran lokasi sppg di Indonesia (fitur peta di website resmi tidak kunjung terbit <html>&#x1F639;</html>) maka dengan sangat malas saya membuat sendiri peta sebaran sppg ini meskipun susah payah mendapatkan sumbernya.
Btw ini sourcenya: https://auditsppg.id/

## Live site

Open the landing page at:
https://thofaa.github.io/sppg/

Click a province from the list to open its dot map or density heatmap.

## Added provinces

- **Aceh** — `aceh_sppg.html` / `aceh_sppg_heat.html`
- **Bali** — `bali_sppg.html` / `bali_sppg_heat.html`

## Contributing

**Verify latitude/longitude data.** The source of truth (mungkin) for every coordinate is the per-province JSON file in `latlong/<province>_sppg.json`. Each entry stores the `sppg_name`, `address`, and the geocoded `lat`/`lon`. Before trusting a coordinate (or before adding a province), open that file and cross-check the `lat`/`lon` values against the address — bad geocoding results are a common issue and worth fixing there, since the maps are generated directly from this file.
