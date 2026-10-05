<!-- tyhp-readme:start -->
# tyhpdef/ramsey-uuid-doctrine

Tyhp type definitions for `ramsey/uuid-doctrine` `2.1.0`.

```bash
composer require --dev tyhpdef/ramsey-uuid-doctrine:2.1.0
```

This is a metapackage. Composer also installs `tyhpdef/ramsey-uuid-doctrine-impl` (type files).
Require **this** name, not `tyhpdef/ramsey-uuid-doctrine-impl`.

See https://tyhplang.com.

## Maintain `ramsey/uuid-doctrine`? Ship the types yourself

If you are a Packagist maintainer of `ramsey/uuid-doctrine`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/ramsey-uuid-doctrine-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `ramsey/uuid-doctrine` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/ramsey-uuid-doctrine": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `ramsey/uuid-doctrine` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `ramsey/uuid-doctrine` with a real constraint,
   `"replace": { "tyhpdef/ramsey-uuid-doctrine": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `ramsey/uuid-doctrine` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/ramsey-uuid-doctrine` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
