# Dotnote

Packaging notes for the Appflare catalog entry.

The public repository commits `app/wrangler.example.jsonc` and does not commit
`app/wrangler.jsonc`. The example file's `database_id` is the source-deploy
placeholder `REPLACE_WITH_D1_DATABASE_ID`. Appflare drops account-specific ids
when it records bindings, and creates a D1 database and an R2 bucket per
install.

`configPatch` rewrites the resource-name vars to the names Appflare actually
creates (`<worker>-bucket`, `<worker>-db`) and removes the example installer
and diagnostics URL. Diagnostics stay off (`DOTNOTE_DIAGNOSTICS_ENABLED` is
already `false` in the example). There is no shared diagnostics token in this
entry.

The Worker's own updater stays idle: it needs a Cloudflare grant that only the
Dotnote installer stores. Appflare is the update path.
