#### [TusinskiDev] Emoji Flags
# td-emoji-flags

A TypeScript package with country and flag emoji constants as Unicode strings.

This library exports named flag emoji values for countries, unions, and additional symbol-based flags such as the United Nations, the rainbow flag, the trans flag, pirate flag, and more.

## Features

- hundreds of country flag emoji constants
- non-country flag symbols
- grouped arrays for convenient filtering and lookup
- works in Node.js and browser-oriented TypeScript code

## Installation

```bash
npm install td-emoji-flags
```

## Usage

```ts
import {
  POLAND_FLAG_EMOJI,
  UNITED_STATES_FLAG_EMOJI,
  UNITED_NATIONS_FLAG_EMOJI,
  RAINBOW_FLAG_EMOJI,
  COUNTRY_FLAGS,
  GEO_FLAGS,
  ALL_FLAGS,
} from 'td-emoji-flags';

console.log(POLAND_FLAG_EMOJI); // 🇵🇱
console.log(UNITED_STATES_FLAG_EMOJI); // 🇺🇸
console.log(UNITED_NATIONS_FLAG_EMOJI); // 🇺🇳
console.log(RAINBOW_FLAG_EMOJI); // 🏳️‍🌈

console.log(COUNTRY_FLAGS.includes(POLAND_FLAG_EMOJI)); // true
console.log(COUNTRY_FLAGS.includes(UNITED_NATIONS_FLAG_EMOJI)); // false
console.log(GEO_FLAGS.includes(UNITED_NATIONS_FLAG_EMOJI)); // true
console.log(ALL_FLAGS.includes(RAINBOW_FLAG_EMOJI)); // true
```

## Exported groups

The package currently exposes these arrays:

```ts
import {
  COUNTRY_FLAGS,
  COUNTRY_UNIONS_FLAGS,
  GEO_FLAGS,
  GENDER_FLAGS,
  OTHERY_FLAGS,
  ALL_FLAGS,
} from 'td-emoji-flags';
```

- `COUNTRY_FLAGS`: country flag emoji strings
- `COUNTRY_UNIONS_FLAGS`: geopolitical and union flags such as the UK, UN, and EU
- `GEO_FLAGS`: combined country + union flags
- `GENDER_FLAGS`: rainbow and trans pride flags
- `OTHERY_FLAGS`: miscellaneous flags and markers like pirate, chequered, and crossed flags
- `ALL_FLAGS`: all emoji flags combined in a single sorted array

## Example constants

```ts
import {
  AFGHANISTAN_FLAG_EMOJI,
  POLAND_FLAG_EMOJI,
  UNITED_STATES_FLAG_EMOJI,
  UNITED_NATIONS_FLAG_EMOJI,
  EUROPEAN_UNION_FLAG_EMOJI,
  RAINBOW_FLAG_EMOJI,
  PIRATE_FLAG_EMOJI,
} from 'td-emoji-flags';
```

## Use cases

- country selectors and dropdown lists with emoji indicators
- dashboards and admin interfaces showing country flags
- UI filters and badges for regional or international data
- emoji-based maps and localization views
- quick access to common flag emojis without maintaining a custom list

## License

MIT
