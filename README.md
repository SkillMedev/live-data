# Live Data

**Free, keyless, liveness-verified APIs for real data - Claude executes instead of deliberating.** — built in-house by [Skill&nbsp;Me](https://skillme.dev).

Reach for this when a task needs real data - weather, geocoding, FX and crypto, earthquakes and NASA imagery, country statistics, dictionary and Wikipedia lookups, trivia, or realistic fake data for a demo - and you want Claude to hit a working free API on the first try instead of deliberating over a directory or reaching for key-walled defaults like OpenWeatherMap and Google Maps from training memory. Each skill names one ranked default per need with exact URL templates, real response shapes with field names and units, and the rate-limit and encoding gotchas that break naive integrations. Every endpoint is probed live (HTTP 200, parseable JSON, under 2s) by a rerunnable health check committed alongside the skills; dead and key-walled APIs are called out by name so they never get cited. A router skill owns the vague 'I need real data for X' trigger and dispatches to the right domain skill. Sourced and liveness-verified from the public-apis project (MIT).

⭐ **If this is useful, star the repo** — it's how we gauge what to build next.

## Install

- **From the catalog:** [skillme.dev/pack/live-data](https://skillme.dev/pack/live-data) — install the whole pack into Claude in one step.
- **With the skills CLI:** `npx skills add SkillMedev/live-data`
- **Manually:** copy any `skills/<slug>/SKILL.md` into your Claude skills directory.

## Skills in this pack

- **[Public Data API Picker](skills/public-data-api-picker/SKILL.md)** — Use when a task needs real, live data but the domain is vague or unstated - "I need real data for X", "is there a free API for this?", "pull actual data into this demo", "no mock data, use a real source", or picking a data source before building.
- **[Weather & Climate Data](skills/weather-climate/SKILL.md)** — Use when a task needs real weather data pulled live - "what's the forecast for X", "current temperature/wind here", "historical weather for this date range", "air quality / AQI right now", or "active US weather alerts" - and you should call a free keyless API instead of deliberating.
- **[Geo & Places Data](skills/geo-places/SKILL.md)** — Use when a task needs live geographic lookups - "geocode this address", "what's at these coordinates" (reverse geocoding), "lat/lon for this city", "which country/state is this ZIP or postal code in", or "country facts: capital, currency, population, flag".
- **[Finance & FX Data](skills/finance-fx/SKILL.md)** — Use when a task needs live or historical money data - "convert USD to EUR", "current/past exchange rate", "FX rate on this date / over this range", or "current price of Bitcoin/Ethereum, market cap, 24h change".
- **[Space & Earth Science Data](skills/space-earth-science/SKILL.md)** — Use when a task needs live space or geophysical data - "recent earthquakes near X / above magnitude Y", "NASA picture of the day", "near-Earth asteroids this week", or "latest full-disk Earth image".
- **[Government & Open Data](skills/government-open-data/SKILL.md)** — Use when a task needs official country-level statistics - "GDP / population / life expectancy / inflation / unemployment for country X over time", "compare indicator Y across countries", or EU-official figures ("Eurostat says…").
- **[Test & Placeholder Data APIs](skills/test-placeholder-data/SKILL.md)** — Use when building a demo, prototype, or tutorial that needs realistic remote data - "fake products/users/todos for this app", "an API I can hit while wiring up fetch", "placeholder images", "seed this UI with something that looks real", or teaching HTTP/CRUD against a live endpoint.
- **[Language & Reference Data](skills/language-reference/SKILL.md)** — Use when a task needs dictionary or encyclopedia lookups from a live source - "define this word", "pronunciation / phonetics / synonyms of X", "get the Wikipedia summary of Y", "search Wikipedia for Z", or pulling a topic's intro paragraph and thumbnail into an app.
- **[Fun Content APIs](skills/fun-content/SKILL.md)** — Use when a task needs light entertainment content from a live API - "build a quiz/trivia game", "random dog picture", "cat fact", "advice of the day", "random fun fact" - for a demo, bot, party feature, or filler content slot.

## License

MIT — see [LICENSE](LICENSE). Skills are portable `SKILL.md` files; the canonical
copies live in the [Skill&nbsp;Me catalog](https://skillme.dev).
