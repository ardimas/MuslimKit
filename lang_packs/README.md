# Language Packs

This folder holds the downloadable translation packs for languages that are **not** bundled into the MuslimKit APK.

## Why this exists

Only 3 languages are compiled directly into the app: **Indonesian (`id`), English (`en`), and Arabic (`ar`)**. The other 12 languages ship as JSON files here instead, and the app downloads the one it needs at runtime — this keeps the APK size down instead of bundling all 15 languages into every install.

```
lang_packs/
  bn.json   Bengali
  de.json   German
  es.json   Spanish
  fr.json   French
  ja.json   Japanese
  ko.json   Korean
  ms.json   Malay
  nl.json   Dutch
  ru.json   Russian
  tr.json   Turkish
  ur.json   Urdu
  zh.json   Chinese
```

## How the app uses these files

When a user selects one of these 12 languages in Settings, the app downloads `lang_packs/<code>.json` from this repo (via `raw.githubusercontent.com`) and caches it locally. On every subsequent app launch, it silently re-downloads that pack in the background (non-blocking, fails silently offline) so that any translation keys added after the user's first download reach them automatically — no manual re-download needed.

**This means:** editing a JSON file in this folder only takes effect for users after the change is actually pushed to the `main` branch of this repo (not just committed locally).

## Format

Flat key-value JSON, UTF-8, one string per app translation key:

```json
{
  "app_name": "MuslimKit",
  "close": "Schließen",
  ...
}
```

## Keeping packs in sync

These files are **generated**, not hand-edited. The source of truth for every language (including the 3 bundled ones) lives in the dev repo at `lib/core/l10n/translations/<code>.dart`. When a translation key is added or changed there, the corresponding JSON file here is regenerated from it and should always end up with the **same key count** as `en.dart`/`id.dart` — if a language's JSON here has fewer keys, either a translation is missing or the file has drifted and needs a resync.
