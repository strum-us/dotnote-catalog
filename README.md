# Dotnote catalog for Appflare

A private Appflare catalog with one app, [Dotnote](https://dotnote.cloud).
Appflare admins add it under **Settings > Catalogs**.

This repository is a copy of [appflare/catalog](https://github.com/appflare/catalog).
Releases are signed with this catalog's own key. The official catalog's key
does not verify them.

## Add it to an Appflare manager

The index is:

```
https://raw.githubusercontent.com/strum-us/dotnote-catalog/main/index.json
```

Paste that URL and this public key into **Settings > Catalogs > Add catalog**:

```
{"keyId":"strum-2026-10","publicKeyBase64":"O0thm1+rZrxYQAiKPDpWL1p/Iulv/FxXvnXGMMMlt/g="}
```

The dialog shows the key's fingerprint. It must be `SHA256:JakF847PAzlX5uFZSjVQ9rgo0iieXe9AzMU8JDVwp4Y` before you save.

## What is listed

| App | Source |
| --- | --- |
| Dotnote | [`strum-us/dotnote`](https://github.com/strum-us/dotnote) `v0.2.10` |

See [TEMPLATE.md](TEMPLATE.md) for how a copy of the official catalog is published.
