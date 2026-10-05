<!-- tyhp-readme:start -->
# tyhpdef/league-csv

Tyhp type definitions for `league/csv` `9.28.0`.

```bash
composer require --dev tyhpdef/league-csv:9.28.0
```

This is a metapackage. Composer also installs `tyhpdef/league-csv-impl` (type files).
Require **this** name, not `tyhpdef/league-csv-impl`.

See https://tyhplang.com.

## Maintain `league/csv`? Ship the types yourself

If you are a Packagist maintainer of `league/csv`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/league-csv-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `league/csv` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/league-csv": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `league/csv` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `league/csv` with a real constraint,
   `"replace": { "tyhpdef/league-csv": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `league/csv` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/league-csv` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
