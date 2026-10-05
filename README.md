<!-- tyhp-readme:start -->
# tyhpdef/behat-behat

Tyhp type definitions for `behat/behat` `3.33.0`.

```bash
composer require --dev tyhpdef/behat-behat:3.33.0
```

This is a metapackage. Composer also installs `tyhpdef/behat-behat-impl` (type files).
Require **this** name, not `tyhpdef/behat-behat-impl`.

See https://tyhplang.com.

## Maintain `behat/behat`? Ship the types yourself

If you are a Packagist maintainer of `behat/behat`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/behat-behat-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `behat/behat` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/behat-behat": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `behat/behat` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `behat/behat` with a real constraint,
   `"replace": { "tyhpdef/behat-behat": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `behat/behat` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/behat-behat` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
