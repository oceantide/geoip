# GeoIP List for V2Ray

Automatically weekly release of `geoip.dat` for V2Ray.

## Download links

- **geoip.dat**：[https://github.com/v2fly/geoip/raw/release/geoip.dat](https://github.com/v2fly/geoip/raw/release/geoip.dat)
- **geoip.dat.sha256sum**：[https://github.com/v2fly/geoip/raw/release/geoip.dat.sha256sum](https://github.com/v2fly/geoip/raw/release/geoip.dat.sha256sum)

## Usage example

```json
"routing": {
  "rules": [
    {
      "type": "field",
      "outboundTag": "Direct",
      "ip": [
        "223.5.5.5/32",
        "119.29.29.29/32",
        "180.76.76.76/32",
        "114.114.114.114/32",
        "geoip:cn",
        "geoip:private"
      ]
    },
    {
      "type": "field",
      "outboundTag": "Proxy-1",
      "ip": [
        "1.1.1.1/32",
        "1.0.0.1/32",
        "8.8.8.8/32",
        "8.8.4.4/32"
      ]
    },
    {
      "type": "field",
      "outboundTag": "Proxy-2",
      "ip": [
        "geoip:us",
        "geoip:ca"
      ]
    },
    {
      "type": "field",
      "outboundTag": "Proxy-3",
      "ip": [
        "geoip:hk",
        "geoip:mo",
        "geoip:tw",
        "geoip:jp",
        "geoip:sg"
      ]
    }
  ]
}
```

## Notice

This product includes GeoLite2 data created by MaxMind, available from [MaxMind](http://www.maxmind.com).

## License

[CC-BY-SA-4.0](https://creativecommons.org/licenses/by-sa/4.0/)
