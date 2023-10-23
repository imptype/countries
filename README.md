# Countries
A collection of metadata about all countries in the world.

### Table of Contents
1. [Information](#1-information)
3. [File Structure](#2-file-structure)
4. [Data Contents](#3-data-contents)
5. [Links and Resources](#4-links-and-resources)
6. [Contributing](#5-contributing)

## 1. Information
Data is arranged by [ISO 3166-1 alpha-2][ISO 3166-1 alpha-2] continent/country codes and [ISO 639-1][ISO 639-1] language codes. However, some more extra languages codes are included with the data too due to [Google][Google Languages], [Steam][Steam Languages] and [Discord][Discord Locales] considering them significant enough:

### 1.1 Localized Languages
> The following language codes below are an [ISO 639-1][ISO 639-1] language code merged with an [ISO 3166-1 alpha-2][ISO 3166-1 alpha-2] country code. So `en` is not present in [`/data/languages.json`](/data/languages.json), we have `en-GB` and `en-US` instead. This doesn't change language speakers distribution maps in [`/maps`](/maps), where only `en.png` is present.
> ```
> en-GB English (US)
> en-US English (UK)
> zh-CN Chinese (Simplified)
> zh-TW Chinese (Traditional)
> pt-BR Portuguese (Brazil)
> pt-PT Portuguese (Portugal)
> ```

### 1.2. Three-Letter Languages
> The following language codes are [ISO 639-2][ISO 639-2] language codes which can be 3 letters in length, and are included in [`/data/languages.json`](/data/languages.json) and language speakers distribution maps in [`/maps`](/maps).
> ```
> bho Bhojpuri
> ceb Cebuano
> doi Dogri
> fil Filipino
> haw Hawaiian
> hmn Hmong
> ilo Ilocano
> kok Konkani
> lus Lushai
> mai Maithili
> mni Meitei
> nso Sepedi
> ```

### 1.3 Three-Letter Languages cont.
> This is the same as above but are an [ISO 639-3][ISO 639-3] language code instead.
> ```
> aem Arem
> ```

### 1.4 Macrolanguages
> The following languages are [macrolanguages][Macrolanguage] stored in [`/data/macrolanguages.json`](/data/macrolanguages.json). They are a derived dialect of a language code in [`/data/languages.json`](/data/languages.json) and have a reference to them in their data. They are not included in language speakers distribution maps in [`/maps`](/maps). Note: Google lists the language code for `Konkani` as `gom`.
> ```
> ckb Kurdish (Sorani) -> ku Kurdish 
> gom Konkani -> kok Konkani 
> kri Kri -> aem Arem
> ```

## 2. File Structure
```
.
├─ data/                      # Contains JSON files
│  ├─ continents.json         # Data about continents
│  ├─ countries.json          # Data about countries
|  ├─ languages.json          # Data about languages + some extras
│  └─ macrolanguages.json     # Data about some macrolanguages
├─ flags/                     # Country flag PNGs
├─ maps/                      # Language speakers distribution PNGs
├─ LICENSE                    # MIT license
└─ README.md                  # Defines this README page
```

## 3. Data Contents
Here is the breakdown of all accessible data in the repository.

### 3.1 Continent
> An example of a continent in [`/data/continents.json`](/data/continents.json):
> ```json
> {}
> ```

### 3.2 Country
> An example of a country in [`/data/countries.json`](/data/countries.json):
> ```json
> {}
> ```

### 3.3 Language
> An example of a language in [`/data/languages.json`](/data/languages.json):
> ```json
> {}
> ```

### 3.4 Localized Language
> An example of a localized language in [`/data/languages.json`](/data/languages.json):
> ```json
> {}
> ```

### 3.5 Macrolanguage 
> An example of a macrolanguage in [`/data/macrolanguages.json`](/data/macrolanguages.json):
> ```json
> {}
> ```

### 3.6 Country Flag
> An example of a country flag in [`/flags`](/flags):
> | `/flags/en.png` or direct URL |
> | - |
> | N/A |

### 3.7 Language Speakers Map
> An example of a language speakers map in [`/maps`](/maps):
> | `/maps/en.png` or direct URL |
> | - |
> | N/A |

## 4. Links and Resources
- [ISO 639-1] - Language codes that are 2 letters in length.
- [ISO 639-2] - Language codes that are 3 letters in length.
- [ISO 639-3] - More language codes that are 3 letters in length.
- [Macrolanguage] - Language codes that can be grouped into a language code above.
- [ISO 3166-1 alpha-2] - Continent and country codes that are 2 letters in length.
- [Google Languages] - List of languages that Google supports.
- [Steam Languages] - List of languages that Steam supports.
- [Discord Locales] - List of languages that Discord supports.

## 5. Contributing
If you have additional information you can / want to share, please, pull requests are welcome!

<!-- Reference Links -->
[ISO 639-1]: https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes
[ISO 639-2]: https://www.loc.gov/standards/iso639-2/php/code_list.php
[ISO 639-3]: https://en.wikipedia.org/wiki/List_of_ISO_639-3_codes
[Macrolanguage]: https://en.wikipedia.org/wiki/ISO_639_macrolanguage
[ISO 3166-1 alpha-2]: https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2
[Google Languages]: https://cloud.google.com/translate/docs/languages
[Steam Languages]: https://partner.steamgames.com/doc/store/localization/languages
[Discord Locales]: https://discord.com/developers/docs/reference#locales
