# MoonBit code mode examples

The standalone script `udp-report.mbtx` reads StatsD metrics from a sample packet capture. A JSON pattern selects outbound records, bit patterns locate the UDP payload, and `lexscan` parses each reading. An enum match adds counters and records the latest gauge value.

Run it with the MoonBit toolchain:

```sh
moonx udp-report.mbtx
```

The sample prints:

```text
counter hits = 5
gauge load = 4
```
