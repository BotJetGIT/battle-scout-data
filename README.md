# Battle Scout data

The data Battle Scout (an Android battle helper for Pokémon Champions doubles) uses for the current regulation set:

- `battle-scout-data.json` — the data pack: the regulation and its dates, ladder usage and sets (PokeTools), Champions move changes, Pokémon and Mega Stones the damage calc doesn't know yet, and how often each Pokémon is brought and led in high-rated games.
- `latest.json` — what the pack holds (regulation, ladder month, when it was built). The app reads this to see whether there's anything new.

The app checks here when it starts (at most every 6 hours) and loads a newer pack by itself. A weekly check publishes a new pack when a regulation set starts or a new month of ladder data comes out. The pack can also be loaded by hand: download `battle-scout-data.json` to the phone, then Battle Scout › Import › Data › Load data pack…

Built by `tools/make_pack.js` in the champions-tools project.
