#### [TusinskiDev] Emoji Flags
# td-emoji-flags

Type-safe country and flag emoji constants for TypeScript, built on top of `td-countries-names`.

This package exports named constants for official country flags and additional Unicode flag-like symbols such as the United Nations, rainbow pride flag, pirate flag, and others.

## Features

- typed country constants using `CountryName`
- official country flag emoji values
- special non-country flag entries
- ready-to-use grouped arrays: `COUNTRY_FLAGS`, `NON_COUNTRY_FLAGS`, and `ALL_FLAGS`
- works in both Node.js and browser-oriented TypeScript projects

## Installation

```bash
npm install td-emoji-flags
```

## Usage

```ts
import {
  POLAND,
  UNITED_STATES,
  UNITED_NATIONS,
  COUNTRY_FLAGS,
  ALL_FLAGS,
} from 'td-emoji-flags';

console.log(POLAND.emoji); // 🇵🇱
console.log(POLAND.name); // Poland
console.log(UNITED_STATES.emoji); // 🇺🇸
console.log(UNITED_NATIONS.emoji); // 🇺🇳

console.log(COUNTRY_FLAGS.length);
console.log(ALL_FLAGS.includes(UNITED_NATIONS));
```

## Use cases

- country selection forms and dropdown lists with emoji indicators
- UI filters for country-specific data and badges
- dashboards and admin panels that display national flags next to names
- localization or user profile views where country names must map to emoji icons
- data normalization when you need a typed country value plus its Unicode flag representation
- special symbol rendering for international or community flags in messaging and apps

## Available exports

```ts
import {
  AFGHANISTAN,
  POLAND,
  UNITED_STATES,
  EUROPEAN_UNION,
  UNITED_NATIONS,
  RAINBOW_FLAG,
  PIRATE_FLAG,
  COUNTRY_FLAGS,
  NON_COUNTRY_FLAGS,
  ALL_FLAGS,
  type Flag,
} from 'td-emoji-flags';
```

The exported constants are immutable objects shaped like this:

```ts
{
  name: 'Poland',
  emoji: '🇵🇱',
}
```

## License

MIT
