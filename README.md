# api-key-avalable-for-free
A field-organized index of legitimate APIs that offer a free tier, with the exact
signup link and the steps to get a working key for each one. Every entry links to the
provider's own signup or docs page — no third-party key resellers, no scraped keys.

Free tiers change often (rate limits get cut, billing gets required, etc.), so treat the
limits listed here as a snapshot and always confirm on the provider's pricing page before
you build something that depends on a specific number.

## Categories

| Folder | Covers |
|---|---|
| [`weather/`](weather/README.md) | Weather and climate data APIs |
| [`maps-geolocation/`](maps-geolocation/README.md) | Maps, geocoding, and location APIs |
| [`ai-llm/`](ai-llm/README.md) | AI / LLM inference APIs |
| [`iot-cloud/`](iot-cloud/README.md) | IoT device-to-cloud and dashboard platforms |
| [`general-misc/`](general-misc/README.md) | News, currency, source control, and other general-purpose APIs |

## How entries are written

Each API entry in the category READMEs follows the same format:

- **What it is** — one line
- **Free tier** — the current limits, as verified on the date noted
- **Sign-up link** — direct link to the provider's own signup/console page
- **Steps to get a key** — the exact click path
- **Notes** — gotchas (activation delay, card requirement, region locks, etc.)

## Contributing

If a link is dead or a free tier has changed, open a PR updating that entry and the
"verified" date next to it.

## License

MIT — see [LICENSE](LICENSE).
