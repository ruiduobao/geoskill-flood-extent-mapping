# geoskill-flood-extent-mapping

See [SKILL.md](SKILL.md) for full usage, inputs and outputs.

## Quick start

```bash
# Local file mode (backward compatible)
python scripts/flood_extent_mapping.py --sar sar.tif
python scripts/flood_extent_mapping.py --sar sar.tif --threshold -16
python scripts/flood_extent_mapping.py --sar sar.tif --output-dir my_output

# Auto-download mode — fetch Sentinel-1 GRD from Microsoft Planetary Computer
# (no API key required; one scene per invocation)
python scripts/flood_extent_mapping.py \
    --bbox 116,39,117,40 \
    --date-range 2024-06-01,2024-06-30 \
    --output-dir my_output
```

## License

MIT
