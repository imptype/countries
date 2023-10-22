# Countries
A collection of metadata about all countries in the world.

### Table of Contents
1. [Information](#1-information)
2. [File Structure](#file-structure)
3. [Data Contents](#data-contents)
4. [Links and Resources](#links-and-resources)
5. [Contributing](#contributing)

## 1. Information
Data is arranged by [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2#DG) continent/country codes and [ISO 639-1](https://en.wikipedia.org/wiki/ISO_639-1) language codes. However, some more extra languages codes are included with the data too due to [Google](https://developers.google.com/custom-search/docs/xml_results_appendices#countryCodes), [Steam](https://partner.steamgames.com/doc/store/localization/languages) and [Discord](https://discord.com/developers/docs/reference#locales) considering them significant enough:

### 1.1 Localized Languages
> The following language codes below are an ISO 639-1 language code merged with an ISO 3166-1 alpha 2 country code. So `en` is not present in `/data/languages.json`, we have `en-GB` and `en-US` instead. This doesn't change language speakers distribution maps in `/maps`, where only `en.png` is present.
> ```
> en-GB English (US)
> en-US English (UK)
> zh-CN Chinese (Simplified)
> zh-TW Chinese (Traditional)
> pt-BR Portuguese (Brazil)
> pt-PT Portuguese (Portugal)
> ```
### 1.2. Three-Letter Languages
> The following language codes are [ISO 639-2](https://www.loc.gov/standards/iso639-2/php/code_list.php) language codes which can be 3 letters in length, and are included in `/data/languages.json` and language speakers distribution maps in `/maps`.
> ```
> bho Bhojpuri
> ceb Cebuano
> doi Dogri
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
> This is the same as above but are an [ISO 639-3](https://en.wikipedia.org/wiki/List_of_ISO_639-3_codes) language code instead.
> ```
> aem Arem
> ```
### 1.4 Macrolanguages
> The following languages are [macrolanguages](https://en.wikipedia.org/wiki/ISO_639_macrolanguage) stored in `/data/macrolanguages.json`. They are a derived dialect of a language code in `/data/languages.json` and have a reference to them in their data. They are not included in language speakers distrubtion maps in `/maps`. Note: Google lists the language code for `Konkani` as `gom`.
```
ckb Kurdish (Sorani) -> ku Kurdish 
gom Konkani -> kok Konkani 
kri Kri -> aem Arem
```
## File structure
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
## Data Contents
An example of a continent in `/data/continents.json`:
```json
{}
```
An example of a country in `/data/countries.json`:
```json
{}
```
An example of a language in `/data/languages.json`:
```json
{}
```
An example of a localized language in `/data/languages.json`:
```json
{}
```
An example of a macrolanguage in `/data/macrolanguages.json`:
```json
{}
```
An example of a country flag in `/flags`:
| `/flags/en.png` or direct URL |
| - |
| N/A |

An example of a language speakers map in `/maps`:
| `/maps/en.png` or direct URL |
| - |
| N/A |
## Links and Resources
- wip
## Contributing
If you have additional information you can / want to share, please, pull requests are welcome!
