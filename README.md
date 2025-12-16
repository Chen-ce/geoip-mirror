# 🌍 GeoIP2 Database Mirror

![Auto Update](https://github.com/Chen-ce/geoip-mirror/actions/workflows/update.yml/badge.svg)
![License](https://img.shields.io/badge/License-CC_BY--SA_4.0-lightgrey)

This repository is an automatic mirror for MaxMind GeoLite2 databases. It updates every **Wednesday** (UTC) via GitHub Actions.

## 📥 Download Links (Always Latest)

Use these links to download the latest databases. They will automatically redirect to the newest release.

| Database | Description | Download Link 🚀 |
| :--- | :--- | :--- |
| **GeoLite2-City** | IP to City/Country | [Download .mmdb](https://github.com/Chen-ce/geoip-mirror/releases/latest/download/GeoLite2-City.mmdb) |
| **GeoLite2-ASN** | IP to ISP/Org | [Download .mmdb](https://github.com/Chen-ce/geoip-mirror/releases/latest/download/GeoLite2-ASN.mmdb) |
| **GeoLite2-Country** | IP to Country | [Download .mmdb](https://github.com/Chen-ce/geoip-mirror/releases/latest/download/GeoLite2-Country.mmdb) |

> **Note:** These are raw `.mmdb` files, extracted and ready to use. No API key required.

## 🛠 Usage in Go

```go
// Example: Download and use directly
const CityURL = "[https://github.com/Chen-ce/geoip-mirror/releases/latest/download/GeoLite2-City.mmdb](https://github.com/Chen-ce/geoip-mirror/releases/latest/download/GeoLite2-City.mmdb)"

func updateDB() {
    resp, _ := http.Get(CityURL)
    // ... save to file ...
}
```

## ⚠️ License & Copyright

This product includes GeoLite2 data created by MaxMind, available from [https://www.maxmind.com](https://www.maxmind.com).

The databases are distributed under the **Creative Commons Attribution-ShareAlike 4.0 International License**.
