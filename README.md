# hokey-lang

Language constants for hokeylization.

`hokey-lang` publishes locale-to-language-name tables as a small ESM package. It currently exports `LOCALE_LANGS`, a record keyed by locale code. Each value is another record mapping language codes to localized language names.

## Install

```sh
pnpm add hokey-lang
```

```sh
npm install hokey-lang
```

## Usage

```ts
import { LOCALE_LANGS } from "hokey-lang";

const englishNames = LOCALE_LANGS.en;
const spanishInEnglish = englishNames.es;
```

The package is ESM-only and includes TypeScript declarations.

## Data Shape

```ts
const LOCALE_LANGS: Record<string, Record<string, string>>;
```

For example, `LOCALE_LANGS.en` contains language names localized in English, and `LOCALE_LANGS.es` contains language names localized in Spanish.

## License

Apache-2.0
