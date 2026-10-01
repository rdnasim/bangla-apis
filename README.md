# Bangla APIs 🇧🇩

> A curated list of free and commercial APIs, SDKs and open datasets for building software in the **Bangladesh** context — payments, couriers, SMS, maps, government services, religion, language and more.

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](#contributing)
![Last reviewed](https://img.shields.io/badge/last%20reviewed-October%202026-blue)

Whether you are building an e-commerce site, a delivery app, a fintech product or a hobby project, this list helps you find the right local service quickly — together with community packages (Laravel, Node.js, Flutter, Python, …) that make integration easier.

---

## Table of Contents

- [How to read this list](#how-to-read-this-list)
- [Payments](#payments)
- [Courier & Logistics](#courier--logistics)
- [SMS & Messaging](#sms--messaging)
- [Maps & Locations](#maps--locations)
- [Government & Identity](#government--identity)
- [Laws & Legal](#laws--legal)
- [Banking & Finance](#banking--finance)
- [Calendar & Holidays](#calendar--holidays)
- [Religious](#religious)
- [News](#news)
- [Telecom & Airtime](#telecom--airtime)
- [Bangla Language & NLP](#bangla-language--nlp)
- [Multi-purpose APIs](#multi-purpose-apis)
- [Integration Tips](#integration-tips)
- [Contributing](#contributing)
- [License](#license)

---

## How to read this list

Every table uses the same columns:

| Column | Meaning |
|---|---|
| **API** | Name of the service, linked to its official website or documentation |
| **Description** | What the API does |
| **Auth** | `No` – open, · `apiKey` – key/token in header or query · `OAuth` – OAuth2 / token grant flow · `Merchant` – credentials issued only after a merchant/business agreement |
| **HTTPS** | Whether the API is served over HTTPS |
| **Pricing** | `Free` · `Freemium` (free tier + paid plans) · `Paid` · `Merchant` (per-transaction fee / contract with the company) |
| **Resources** | Official SDKs, community packages, examples and docs |

Status markers:

- ⚠️ — the service or link could not be reached during the last review and may be offline or moved. Please verify before relying on it (and send a PR if you know the new URL!).
- 📦 — not a hosted API but an open dataset / library you can self-host.

---

## Payments

| API | Description | Auth | HTTPS | Pricing | Resources |
|---|---|---|---|---|---|
| [bKash](https://developer.bka.sh/) | Largest mobile financial service (MFS) in Bangladesh. Checkout (URL based), Tokenized Checkout (agreement based), refund, search & payout APIs with sandbox | Merchant | Yes | Merchant | [Official GitHub](https://github.com/bKash-developer), [API reference](https://developer.bka.sh/reference), [flutter_bkash](https://pub.dev/packages/flutter_bkash), [laravel-bkash-tokenize](https://github.com/karim-007/laravel-bkash-tokenize) |
| [Nagad](https://nagad.com.bd/) | Accept payments from Nagad wallets. API docs & sandbox credentials are shared with registered merchants | Merchant | Yes | Merchant | [laravel-nagad](https://github.com/codeboxrcodehub/nagad), [nagadApi (PHP)](https://github.com/arif98741/nagadApi), [node-nagad](https://github.com/shahriar-shojib/nagad-payment-gateway), [community docs](https://github.com/theshakhawat/nagad-payment-gateway-documentation) |
| [Upay](https://www.upaybd.com/) | Accept payments from Upay (UCB Fintech) wallets | Merchant | Yes | Merchant | [laravel-upay](https://github.com/codeboxrcodehub/upay) |
| [SSLCOMMERZ](https://developer.sslcommerz.com/) | Aggregated payment gateway — cards, internet banking and MFS (bKash, Nagad, Rocket, Upay…) behind one API, with IPN & sandbox | Merchant | Yes | Merchant | [Official GitHub](https://github.com/sslcommerz) |
| [aamarPay](https://developer.aamarpay.com/) | Payment gateway that redirects customers to a hosted aamarPay checkout; cards and wallets | Merchant | Yes | Merchant | [Official GitHub](https://github.com/aamarpay-dev), [Flutter](https://github.com/aamarpay-dev/aamarPay-flutter), [Android](https://github.com/aamarpay-dev/aamarPay-Android-Library) |
| [shurjoPay](https://shurjopay.com.bd/) | Bangladesh Bank licensed gateway — online payments, QR payments and payment links | Merchant | Yes | Merchant | [Developer docs](https://shurjopay.com.bd/developers), [Plugins & examples](https://github.com/shurjopay-plugins/sp-plugin-usage-examples), [Laravel](https://github.com/smukhidev/shurjopay-laravel-package), [Android](https://github.com/smukhidev/android-sdk), [Flutter](https://github.com/smukhidev/fluttre) |
| [PortPos](https://portpos.com/) | Online payment acceptance, invoices and payment links | Merchant | Yes | Merchant | [Developer docs](http://developer.portpos.com/) |

## Courier & Logistics

| API | Description | Auth | HTTPS | Pricing | Resources |
|---|---|---|---|---|---|
| [Pathao Courier](https://merchant.pathao.com/) | Merchant API to create stores & orders, fetch cities/zones/areas, calculate price and track parcels. Sandbox: `courier-api-sandbox.pathao.com`, live: `api-hermes.pathao.com` | OAuth | Yes | Merchant | [WooCommerce plugin (official)](https://github.com/pathao-eng/courier-woocommerce-plugin), [Laravel](https://github.com/enuenan/pathao-courier), [Python](https://github.com/mojnomiya/pathao-python), [Node.js/TS](https://github.com/Sifat07/pathao-merchant-sdk) |
| [Steadfast Courier](https://steadfast.com.bd/) | Create single / bulk orders, check delivery status and balance. Base URL: `portal.packzy.com/api/v1` | apiKey | Yes | Merchant | [WordPress plugin](https://wordpress.org/plugins/steadfast-api/) |
| [RedX](https://redx.com.bd/) | Create parcels, look up areas and track parcels | apiKey | Yes | Merchant | [Laravel](https://github.com/codeboxrcodehub/redx-courier) |
| [Paperfly](https://paperfly.com.bd/) | Parcel booking and order tracking. Base URL: `api.paperfly.com.bd` | apiKey | Yes | Merchant | — |
| [eCourier](https://ecourier.com.bd/) | On-demand last-mile delivery network with merchant & reseller APIs | apiKey | Yes | Merchant | [General API doc (PDF)](https://ecourier.com.bd/wp-content/uploads/eCourier_Merchant_API_Document_General_v5.2.pdf), [Reseller API doc (PDF)](https://ecourier.com.bd/wp-content/uploads/eCourier_Merchant_APIDocument__Reseller_v5.2.pdf), [Laravel](https://github.com/codeboxrcodehub/ecourier-courier), [WordPress tracker](https://github.com/simongomes/ecourier-parcel-tracker), [WooCommerce](https://github.com/simongomes/ship-to-ecourier) |
| [pandago](https://pandago-bd.com/) | On-demand delivery of food, documents, parcels and gifts (by foodpanda) | OAuth | Yes | Merchant | [API docs](https://pandago.docs.apiary.io/), [Laravel SDK](https://github.com/lloricode/laravel-pandago-sdk) |

> 💡 **Multi-courier:** [arif98741/multicourier](https://github.com/arif98741/multicourier) is a Laravel library with a single interface for eCourier, Pathao, Steadfast, RedX and more.

## SMS & Messaging

Most Bangladeshi SMS providers require a registered account and (for masking) BTRC-approved sender IDs.

| API | Description | Auth | HTTPS | Pricing | Resources |
|---|---|---|---|---|---|
| [BulkSMSBD](https://bulksmsbd.com/bulksms-api-bangladesh.php) | Bulk / OTP SMS API with one-to-many and many-to-many JSON endpoints | apiKey | Yes | Paid | [GitHub topic](https://github.com/topics/bulksmsbd) |
| [Alpha SMS](https://www.alpha.net.bd/sms/) | Bulk SMS, OTP, masking and non-masking SMS API | apiKey | Yes | Paid | — |
| [SMS.NET.BD](https://sms.net.bd/) | Bulk SMS & OTP API (sister service of Alpha Net) | apiKey | Yes | Paid | — |
| [SSL Wireless](https://sslwireless.com/) | Enterprise SMS gateway (v2 & v3 APIs) used by many banks and large brands | apiKey | Yes | Paid | — |
| [MiM SMS](https://www.mimsms.com/) | Bulk SMS gateway & API | apiKey | Yes | Paid | — |
| [GreenWeb SMS](https://greenweb.com.bd/) | Bulk SMS API popular with small businesses | apiKey | Yes | Paid | — |

> 💡 **Multi-provider:** [sarahman/sms-service-with-bd-providers](https://github.com/sarahman/sms-service-with-bd-providers) wraps several BD SMS gateways (SSL, GreenWeb, BulkSMSBD, Alpha…) behind one Laravel interface.

## Maps & Locations

| API | Description | Auth | HTTPS | Pricing | Resources |
|---|---|---|---|---|---|
| [Barikoi](https://docs.barikoi.com/) | Bangladeshi location platform — autocomplete, geocoding, reverse geocoding, nearby, distance, routing and the *Rupantor* address parser | apiKey | Yes | Freemium | [Business API](https://docs.barikoi.com/api/), [Laravel / PHP](https://packagist.org/packages/barikoi/barikoiapis), [Go](https://github.com/barikoi/barikoiapis-golang), [Postman](https://documenter.getpostman.com/view/2611089/RWTmvdtF) |
| [Dingi Maps](https://www.dingi.tech/api.php) | Maps, search, autocomplete and reverse geocoding with a free tier | apiKey | Yes | Freemium | [API docs](https://www.dingi.tech/docs/api/index.html), [Web sample](https://github.com/dingilive/map-integration-web/blob/master/map_view.html), [Android SDK](https://www.dingi.tech/docs/android-sdk/index.html), [iOS SDK](https://www.dingi.tech/docs/ios-sdk/index.html) |
| [BD API](https://bdapis.com/) | Divisions, districts, upazilas, thanas, post offices & post codes in Bangla and English. *(Moved from the old `bdapis.herokuapp.com`)* | No | Yes | Free | [GitHub](https://github.com/AbmSourav/bdapis), [RapidAPI](https://rapidapi.com/AbmSourav/api/bdapi) |
| [bangladesh-geocode](https://github.com/nuhil/bangladesh-geocode) 📦 | Division → District → Upazila → Union dataset in SQL, CSV, JSON, XML & PHP, plus GeoJSON | No | Yes | Free | [JSON files](https://github.com/nuhil/bangladesh-geocode/tree/master/divisions) |
| [bangladesh-geojson](https://github.com/ifahimreza/bangladesh-geojson) 📦 | GeoJSON boundaries for divisions, districts and upazilas | No | Yes | Free | — |
| [bd-apis](https://github.com/SudipMHX/bd-apis) | Lightweight self-hostable REST API for divisions, districts and upazilas | No | Yes | Free | — |

## Government & Identity

| API | Description | Auth | HTTPS | Pricing | Resources |
|---|---|---|---|---|---|
| [Porichoy](https://porichoy.gov.bd/) | Real-time NID-based identity (KYC) verification gateway | Merchant | Yes | Paid | [npm](https://www.npmjs.com/package/porichoy) |

## Laws & Legal

| API | Description | Auth | HTTPS | Pricing | Resources |
|---|---|---|---|---|---|
| [BD Laws API](https://bd-laws.pages.dev/) ⚠️ | Community API for the Laws of Bangladesh — search, volumes, acts and sections | No | Yes | Free | [search](https://bd-laws-api.bdit.community/api/search/dhaka), [volumes](https://bd-laws-api.bdit.community/api/volumes), [acts](https://bd-laws-api.bdit.community/api/acts/1), [sections](https://bd-laws-api.bdit.community/api/sections/28) |
| [bdlaws (Ministry of Law)](http://bdlaws.minlaw.gov.bd/) | Official, authoritative source of Bangladeshi statutes (website, no public API) | No | — | Free | [Hugging Face dataset](https://huggingface.co/datasets/Ashik2380/bdlaws) 📦 |

## Banking & Finance

| API | Description | Auth | HTTPS | Pricing | Resources |
|---|---|---|---|---|---|
| [BD-Bank-List](https://github.com/khyrulAlam/BD-Bank-List) 📦 | List of banks operating in Bangladesh | No | Yes | Free | [GitHub](https://github.com/khyrulAlam/BD-Bank-List) |
| [Frankfurter](https://frankfurter.dev/currencies/bdt/) | Free, open-source exchange-rate API with current & historical BDT rates (e.g. `api.frankfurter.dev/v2/rate/bdt/usd`) | No | Yes | Free | [Docs](https://frankfurter.dev/) |

## Calendar & Holidays

| API | Description | Auth | HTTPS | Pricing | Resources |
|---|---|---|---|---|---|
| [Holiday API](https://holidayapi.com/docs) | Public holidays and observances for many countries, including Bangladesh | apiKey | Yes | Freemium | — |
| [Doptor Portal Holiday API](https://doptor-portal.tappware.com/blog/holiday-calendar-api) | Government holiday calendar of Bangladesh from the Doptor (e-Nothi) platform | apiKey | Yes | Free | — |

> ℹ️ [Nager.Date](https://date.nager.at/) is a popular free holiday API, but it currently has **no data for Bangladesh**.

## Religious

| API | Description | Auth | HTTPS | Pricing | Resources |
|---|---|---|---|---|---|
| [Bangla Quran API](https://github.com/alQuranBD/Bangla-Quran-api) | Holy Quran with Bangla and English translation, including *Tafhimul Quran* tafseer | No | Yes | Free | [GitHub](https://github.com/alQuranBD/Bangla-Quran-api) |
| [Bangla Hadith API](https://github.com/alQuranBD/Bangla-Hadith-api) | Large Hadith collection from multiple books in Arabic, Bangla and English | No | Yes | Free | [GitHub](https://github.com/alQuranBD/Bangla-Hadith-api) |
| [Quran.com API](https://github.com/quran/quran.com-api) | The API behind Quran.com — recitations, translations (incl. Bangla) and tafsir | No | Yes | Free | [Docs](https://quran.api-docs.io/v3) |
| [AlAdhan](https://aladhan.com/prayer-times-api) | Prayer times, Hijri calendar and Qibla direction. Example: `api.aladhan.com/v1/timingsByCity?city=Dhaka&country=BD&method=1` | No | Yes | Free | [OpenAPI spec](https://api.aladhan.com/v1/documentation/openapi/prayer-times/yaml), [PHP client](https://packagist.org/packages/aladhan/api-client), [Python](https://pypi.org/project/aladhan-api) |

## News

| API | Description | Auth | HTTPS | Pricing | Resources |
|---|---|---|---|---|---|
| [Latest Bangladesh News](https://gnewsapi.net/pages/bd/bn.html) ⚠️ | Latest Bangladesh news in Bangla (বাংলা) | No | Yes | Free | [gnewsapi](https://gnewsapi.net/) |

## Telecom & Airtime

| API | Description | Auth | HTTPS | Pricing | Resources |
|---|---|---|---|---|---|
| [Reloadly Airtime](https://operators.reloadly.com/grameenphone-robi-banglalink-teletalk-bangladesh-airtime-api/) | Mobile top-up for Grameenphone, Robi, Banglalink and Teletalk | OAuth | Yes | Freemium | — |

## Bangla Language & NLP

Open-source libraries and models (📦 — self-hosted) for working with Bangla text.

| Project | Description | Auth | HTTPS | Pricing | Resources |
|---|---|---|---|---|---|
| [BNLP](https://github.com/sagorbrur/bnlp) 📦 | Bangla NLP toolkit — tokenization, embeddings, POS tagging, NER | No | — | Free | `pip install bnlp_toolkit` |
| [BanglaBERT](https://github.com/csebuetnlp/banglabert) 📦 | Pre-trained Bangla language model from BUET CSE NLP group, with fine-tuning code & benchmarks | No | — | Free | [Hugging Face](https://huggingface.co/csebuetnlp/banglabert) |
| [BNLTK](https://github.com/ashwoolford/bnltk) 📦 | Bangla Natural Language Toolkit — tokenizer, stemmer, POS tagger | No | — | Free | [PyPI](https://pypi.org/project/bnltk) |

## Multi-purpose APIs

| API | Description | Auth | HTTPS | Pricing | Resources |
|---|---|---|---|---|---|
| [BDApi4All](https://github.com/fakhrul62/bdapi4all) | One open REST API for BD geography, prayer times, holidays, exchange rates, mobile operators, validators, Bengali utilities and more. Base URL: `bdapi4all.vercel.app/api/v1` | No (optional `X-API-Key`) | Yes | Free | [GitHub](https://github.com/fakhrul62/bdapi4all) |

---

## Integration Tips

- **Always start in sandbox.** bKash, Nagad, SSLCOMMERZ, aamarPay, shurjoPay and Pathao all provide sandbox credentials — never test with live keys.
- **Verify payments server-side.** Don't trust the success redirect alone; confirm the transaction with the gateway's *validate / query / IPN* endpoint before fulfilling an order.
- **Keep secrets on the server.** API keys, merchant passwords and private keys must never ship in a mobile app or frontend bundle.
- **Whitelisting.** Several gateways (e.g. Nagad) require your server's public IP to be whitelisted — plan for a static IP.
- **SMS compliance.** Masked sender IDs and promotional SMS are regulated by BTRC; register your sender ID with your provider.

---

## Contributing

Contributions are very welcome! To add or update an API:

1. Fork the repo and create a branch from `develop`.
2. Add your entry to the right section, **keeping the table format** and alphabetical/logical order:

   ```md
   | [Name](https://link-to-docs) | Short description | apiKey | Yes | Free | [package](https://link) |
   ```

3. Use the values defined in [How to read this list](#how-to-read-this-list) for *Auth* and *Pricing*.
4. Prefer official documentation links; add community packages under *Resources*.
5. If you find a dead link, mark it with ⚠️ or replace it with the new URL.
6. Open a pull request with a short description of your change.

Ideas for missing categories: **Rocket / Pathao Pay / Tap payment APIs, e-commerce fraud check, education board results, BRTA, weather (BMD), stock market (DSE/CSE)** — PRs welcome!

---

## License

This list is shared for the benefit of the Bangladeshi developer community. Each API is owned by its respective provider and subject to its own terms of service.
